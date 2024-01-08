# Основные git команды
## **Описание и основные отличия команд git pull и git fetch**

Команды git pull и git fetch используются для обновления локального репозитория (чтобы скачать последние коммиты).

## **git pull** 
Эта команда объединяет в себе git fetch и git merge. Т.е. когда вы обновляете локальный репозиторий с помощью git pull, то все изменения не просто будут скачены, а еще и внедрятся (объединятся) в ваш локальный репозиторий. Другими словами эта команда обновит ваш локальный репозиторий до состояния на сервере.

## **git fetch** 
Эта команда скачивает обновления из удаленного репозитория, но не сливает их с текущей веткой. Другими словами вы скачаете новые коммиты, но не добавите их в историю изменений локального репозитория. Для завершения процесса обновления нужно будет сделать еще git merge. Эта операция безопасна для выполнения в любое время т.к. она не вносит изменения в локальную ветку.

## **git commit --amend** 
Эта команда помогает изменить последний коммит. Она позволяет объединить проиндексированные изменения с предыдущим коммитом без создания нового коммита. Ее можно использовать для редактирования комментария к предыдущему коммиту без изменения состояния кода в нем. Но такое изменение не только редактирует последний коммит, но и полностью его заменяет. То есть измененный коммит станет новой сущностью с отдельной ссылкой.

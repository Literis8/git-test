# 1. Системы контроля версий
## 1.1 Системы управления версиями

Checkout - извлечение версии

Состояния фала в Git:
* Зафиксированный (committed) - файл уже сохранен в локальной базе
* Измененный (modified) - файлы которые изменились, но еще не зафиксированны
* Подготовленный (staged)  измененные файлы, отмеченные для включения в следующий коммит.
## 1.2 Начало работы с Git
`git config --system ` - системная конфигурация (/etc/gitconfig)

`git config --global` - конфигурация пользователя (~/.gitconfig/ или ~/.config/git/config)

`git config --local` - конфигурация в репозитории (./git/config)

`git config --list --show-origin` -  посмотреть все настройки и где они заданы.

`git config --global user.name “Eugeni.Sai”` - установить имя пользователя

`git config --global user.email literis8@gmail.com` - установить электронную почту

`git init` - создать пустой репозиторий в текущей директории

`git add <file>` - взять файл под контроль версий. (staged)

`git commit -m “message”` - выполнить коммит добавив сообщение “message” 

`git clone <url> <dir>` - склонировать репозиторий по url в директорию dir

`git status` - показать какие файлы в каком состоянии находятся.

`git status -s` - (--short) упрощенный вывод статуса

`./.gitignore` - список файлов которые не должны попасть в репозиторий.

https://github.com/github/gitignore - набор различных шаблонов gitignore

`git diff --staged` - отобразить изменения файлов staged

`git push` - отправка изменений в репозиторий

https://guides.github.com/features/mastering-markdown/ - краткое описание языка markdown

# 2. Основы Git
## 2.1 Работа с историей изменений файлов Git
`git diff` - отобразить непроиндексированные изменения файлов modified

`git diff --staged` `git diff --cached`- отобразить проиндексированные изменения файлов staged с последним коммитом

`git difftool` - графическая утилита для сравнения изменений

`git commit -v` - добавить в комментарий коммита diff

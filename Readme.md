# Инструкция по работе с Git и ветками

## Что такое Git
Git - это наиболее популярная реализация распределенной системы контроля версий. Самая популярная реализация **Git** - это [GitHub](http:??github.com/)
## Подготовка репозитория
Для создания репозитория используется команда *git init*, Для этого необходимо в терменале перейти в пустую папку, где в будущем будет репозиторий. Затем в терменале с папкой написать команду *git init*. 
## Создание коммита
Для создания коммита используется команда *git commit*. Для этого в терминале с папкой-репозиторием необходимо написать *git commit -m <сообщение к коммиту>*. Сообщение к коммиту писать ***ОБЯЗАТЕЛЬНО!!!*** 

### Добавление фaйла к коммиту
Для добавления файла к будущему коммиту используется команда *git add*. Для этого в терменале с папкой-репозиторием необходимо написать *git add <название файла>*.

## Перемещение между коммитами
Для перемещения на предыдущие коммиты используется команда *git checkout*. Для этого необходимо в журнале изменений найти необходимый коммит и его номер. После чего в иерменале с папкой-ркпозиторием написать команду *git  checkout <номер коммита>*. после применения этой команды вы попадете в состояние *Detached head*, в котором никакие изменения фиксироваться не будут. Для возврата в обычное состояние необходимо написать команду *git checkout master*. 
## Журнал изменений
Для просмотра журнала изменений используется команда *git log*. Для этого в терменале с папкой-репозиторием необходимо написать *git log*. 

## Ветки в Git
Под веткой приянто понимать независимую последовательность коммитов в хронологическом порядке. Имя основной ветки Git-проекта по умолчанию - master, она появляется сразу при инициализации репозитория. 
Команда *git branch* - главный инструмент для работы с ветвлением. С ее помощью можно добавлять новые ветки, перечислять и переименовывать существующие и удалять их. 
### Создание веток в Git
Для создания новой ветки в Git используется 
*git branch*. Для этого в терминале с пакой-репозиторием необходимо написать команду *git branch <название ветки>*.
### Просмотр списка веток
Для просмотра списка веток используется команда *git branch*. Для этого в ткрминале с паакой-репозиторием необходимо написать команду *git branch*. Зеленым цветом с символом **звездочка** дудет выделена текущая ветка. 
Для получения списка удаленных веток используем *-r*/
Для вывода удаленных и локальных веток используем *-a*/
### Слияние веток
Для переноса изменений с одной ветки на другую используем команду *git merge *name of merge branch*. При этом данная операция может привести к появлению конфликтов.
### Разрешение конфликтов
Решить конфликты можно двумя способами:
1. вручную разрешить файловый конфликт. Для этого нужно самим изменить файлы, с которыми возникли проблемы.
2. Выбрать более подходящий файл, от второго отказаться. 
### Переименование ветки. 
Для тго, чтобы переименовать ветку используем команду: git branch -m *new name of branch*.
### Удаление ветки
Для удаления ветки исползуем команду: git branch -d *name of branch*/
### Дерево веток
Для графического представления ветвей прямо в терминале используем команду: git log --graph.


## Слияние веток и разрешение конфликтов
Для переноса изменений с одной ветки на другую используем команду *git merge *name of merge branch*. При этом данная операция может привести к появлению конфликтов.
### Разрешение конфликтов
Решить конфликты можно двумя способами:
1. вручную разрешить файловый конфликт. Для этого нужно самим изменить файлы, с которыми возникли проблемы.
2. Выбрать более подходящий файл, от второго отказаться. 
## Удаление веток
Для удаления ветки исползуем команду: git branch -d *name of branch*.

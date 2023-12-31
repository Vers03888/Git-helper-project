# Шпаргалка по Git

## Навигация в командной строке

1. `pwd` - команда, которая выводит в текущую директорию, там где мы сейчас.
2. `cd ~` - команда, которая выводит в домашнюю директорию.
3. `ls` - команда, которая выводит содержимое директории.
4. `cd` - команда, которая сменяет текущую директорию.
5. `cd ..` - команда, которая сменяет текущую директорию на уровень выше.
6. `cd .` - команда, которая обращается к текущей директории.
7. `cd dir/dir` - команда, которая сменяет текущую директорию через несколько папок.
8. `ls -a` - команда, которая выводит содержимое директории вместе со скрытыми файлами и папками.
9. `ls ~` - команда, которая выводит содержимое домашней директории.
10. `ls ..` - команда, которая выводит содержимое родительской директории.
11. `cd /` - команда, которая выводит в корневую директорию.


## Хеш идентификатор коммита

_Хеширование_ - это способ преобразовать набор данных и получить их отпечаток.
* `git log --oneline` - команда получить сокращенный лог.
* `cat HEAD` - команда для получения ссылки на последний коммит refs/heads/master.
* `cat refs/heads/master` - получаем хеш последнего коммита.

HEAD -- это голова.
Коммит -- это всему голова.
Статусы файлов:

```mermaid
graph LR;
  untracked -- "git add" --> staged;
  staged    -- "git commit -m"     --> tracked/comitted;

%% стрелка без текста для примера: 
  A --> B;
```
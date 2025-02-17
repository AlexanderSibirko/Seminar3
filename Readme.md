# Инструкция по работе с Git и GiHub

## Что такое Git?
**Git** - одна из реализаций распределённых систем контроля версий. Позволяет контролировать версионность файлов как локально, так и на удалённом сервере. Самая популярная система контроля версий

Скчать можно [тут](https://git-scm.com/).

## Подготовка репозитория
**Репозиторий** - это хранилище файлов, поддреживающее версионность. Создать репозиторий в папке можно с помощью команды *git init*, применив эту команду в папке с будущим репозиторием.

## Создание "сохранений"
Создать "сохранения" они же фиксации или коммиты, мы можем с помощью команды *git commit*. Для этого необходимо написать команду *git commit -m <сообщение к коммиту>* сообщение к коммиту писать **ОБЯЗАТЕЛЬНО**. Все файлы должны быть добавлены в коммит с помощью команды *git add*. Если файлы не добавлены, то можно использовать флаг *-a* и команда преобретёт вид *git commit -a -m "<сообщение к коммиту>*.

## Журнал изменений

## Перемещение между "сохранениями"
Для переключения между "сохранениями"(коммитами), необходимо использовать команду *git checkout* следующим образом: *git checkout <номер коммита для переключения>*. Номер коммита берётся из истории коммитов и на него произойдёт переключение.

Команды *git reset* и *git revert* позволяют отменять изменения. Команда *git revert* возвращает к указанному коммиту, создавая новый коммит, а команда *git reset* возвращает к указанному коммиту и затирает историю изменений до указанного коммита. Применяется это следующим образом: *git revert <номер коммита>* или *git reset --hard <номер коммита>* 

## Ветки в Git
Ветки в Git позволяют создавать разветвления, то есть работать с одним и тем же содержимым в разных его версиях. Посмотреть список имеющихся веток можно с помощью команды *git branch*, а создать новую ветку из текущей можно с помощью команды *git brnach <имя ветки>*.

## Слияние веток и решение конфликтов


## Удаление веток
Для того, чтобы удалить уже слитую ветку используется команда *git branch -d <имя ветки>*

## Скачивание удалённого репозитория
Слияние веток происходит с помощью команды *git clone*. Для этого в удобной папке надо написать *gity clone <адрес репозитория>*.


## Отправка изменений в удалённый репозиторий
Отправить изменения в удалённый репозиторий можно с помощью команды *git push*. Для этого примените в папке с репозиторием команду *git push origin <название ветки>* для отправки изменений в куазанную ветвеь. По умолчанию в название ветки лучше всего писать **master**

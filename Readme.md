# Инструкция по работе с GIT


## Что такое Git?

## Подготовка репозитория
Для того, чтобы создать репозиторий используется команда *git init*. Для этого необходимо написать в терминале в папке будущего репозитория *git init*

## Создание "сохранений"

### Добавление файла коммиту

Для добавления файла к коммиту используется команда *git add*. Пишется она следующим образом *git add <имя файла>* в терминале в папке с созданным репозиторием.

### Создание коммита

Для создания нового "сохранения" используется команда *git commit*. Используется она следующим образом: в терминале с папкой-репозиторием пишется *git commit -m <сообщение коммиту>*. Сообщение коммиту писать **обязательно** 


## Журнал изменений

Для просмотра журнала изменений испульзуется команда *git log*. Для этого в терминале в папке с репозиторием достаточно написать *git log*.

## Перемещение между коммитами

Для  перемещения между сохранениями используется команда *git checkout*. Для того, чтобы переместиться на указанный коммит в терминале в папке с репозиторием пишем *git checkout <номер коммита>*. **Номер коммита** берется из журнала изменений, о котором сказано выше. После перемещения на указанный коммит мы попадаем в состояние **detached head**. Чтобы вернуться к обычной работе, необходимо написать *git checkout master*.


## Ветки в GIT
Создать ветку в Git можно способом: команда "git branch <имя новой ветки>" .
Ветка в GIT - это шкала последовательных коммитов, то есть является местом повседневной работы разработчиков. Ветка может быть основной, то есть она будет отражаться в основном пути развития программы.

## Слияние веток и разрешение конфликтов

## Удаление веток
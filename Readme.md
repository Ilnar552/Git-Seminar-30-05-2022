# Инструкция по работе с Git и удаленными репозиториями


## Что такое Git?
Распределенная система управление версиями. Прект был создан Линусом Торвальдсом для управления разработкой ядра Linux, первая выпущена в 7 апреля 2005 года. На сегодняшний день его поддерживает Джунио Хамано.
*Git* -  одна из реализаций распределенных систем контроля версий. *Git* на данный момент является самой популярной реализацией. Самой популярной реализацией *Git* является [GitHub](https://github.com)

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
Ветки в *Git* нужны для того чтобы работать с *черновиком* и с *чистовиком*. Для того, чтобы создать новую ветку используется команда *git branch*. В терминале в папке с репозиторием, напишите *git branch <название ветки>*

## Слияние веток и разрешение конфликтов
Для слияние двух веток используется команда *git merge*. Для её использования необходимо перейти в ту ветку, куда вы хотите сделать слияние. После чего в терминале в папке репозитория написать *git merge <название ветки>*. Чаще всего слияние происходит автоматически, но возможно **КОНФЛИКТЫ** в таком случае, необходимо вручную получить желаемую версию файла и сделать коммит.  

## Удаление веток
Чтобы удалить локальную ветку в GIT нужно выполнить команду "git branch -d <имя ветки>". Обратите внимание на то, что ветка, которую удалаетк, не должна быть вашей текущей веткой, в которой вы работаете, иначе отобразится ошибка вида: error:Cannot delete branch <имя ветки>.

## Получение удаленного репозитория

## Скачивание изменений с удаленного репозитория

## Отправка изменений в удаленный репозиторий
# Инструкция для работы с Git и удалёнными репозиториями

## Что такое Git?
Git - это одна из реализаций распределённых систем контроля версий, имеющая как и локальные, так и удалённые репозитории. Является самой популярной реализацией систем контроля версий в мире.

## Установка

Установим сам Git.

* Windows. Проходим по этой [ссылке](https://git-scm.com/download/win), выбираем под вашу ОС (32 или 64 битную), скачиваем и устанавливаем.

* Для Mac OS. Открываем терминал и пишем:

```
#Если установлен Homebrew
brew install git

#Если нет, то вводим эту команду. 
git --version
#После этого появится окно, где предложит установить Command Line Tools (CLT).
#Соглашаемся и ждем установки. Вместе с CLT установиться и git
```

## Как работает
> Если посмотреть на картинку, то становиться чуть проще с пониманием. Каждый кружок, это commit. Стрелочки показывают направление, из какого commit сделан следующий. Например C3 сделан из С2 и т. д. Все эти commit находятся в ветке под названием main. Это основная ветка, чаще всего ее называют master . Прямоугольник main* показывает в каком commit мы сейчас находимся, проще говоря указатель.

![enter image description here](image_one.png)

## Подготовка репозитория
Для создание репозитория необходимо выполнить команду *git init*  в папке с репозиторием и у Вас создаться репозиторий (появится скрытая папка .git)

## Создание коммитов

### Git add
Для добавления измений в коммит используется команда *git add*. Чтобы использовать команду *git add* напишите *git add <имя файла>*

### Просмотр состояния репозитория
Для того, чтобы посмотреть состояние репозитория используется команда *git status*. Для этого необходимо в папке с репозиторием написать *git status*, и Вы увидите были ли измения в файлах, или их не было.

### Создание коммитов
Для того, чтобы создать коммит(сохранение) необходимо выполнить команду *git commit*. Выполняется она так: *git commit -m "<сообщение к коммиту>*. Все файлы для коммита должны быть ***ДОБАВЛЕНЫ*** и сообщение к коммиту писать ***ОБЯЗАТЕЛЬНО***.

## Перемещение между сохранениями
Для того, чтобы перемещаться между коммитами, используется команда *git checkout*. Используется она в папке с пепозиторием следующим образом: *git checkout <номер коммита>*

## Журнал изменений
Для того, чтобы посмтреть все сделанные изменения в репозитории, используется команда *git log*. Для этого достаточно выполнить команду *git log* в папке с репозиторием

## Ветки в Git
Пробуем комиты
~~ Мой текст ~~
### Создание ветки

Для того, чтобы создать ветку, используется команда *git branch*. Делается это следующим образом в папке с репозиторием: *git branch <название новой ветки>*

## Слияние веток

Для того чтобы дабавить ветку в текущую ветку используется команда *git merge <name branch>*

## Удаление веток
Для удаления ветки ввести команду "git branch -d 'name branch'"

## git add
Создала свою ветку newBranch. Вношу изменения в файл, чтобы потом слить эти изменения в основную ветку. 

## Домашнаяя работа с гитом
Создала ветку hw1 - в ней удалила лишнюю строку с занятия. Сейчас нахожусь в ветке hw2, пишу это описание. 

## Merge conflicts
Стою на ветке hw4. Добавляю строки там же что и в ветке hw3. L Для решения конфликтов оставлю оба изменения
Создала ветку hw3, вношу здесь этот текст - дальше в hw4  буду изменять эти де строки для создания конфликта. 

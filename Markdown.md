  # Инструкция для работы с Markdown
  22.12.2022
 новая попытка создать конфликт
  ## Выделение текста

  Чтобы выделить текст курсивом 
  необходимо обрамить его звездочками
  (*). Например, *вот так*.

  чтобы выделить текст полужирным
 необходимо обрамить его 

  ## Списки

 ## Работа с изображениями

 Чтобы вставить изображение в текст, 
 достаточно написать следующее:

![algoritm](18.png)

 * Git idit - иницилиазирует гит в папке
* Git add - добавляет файл к отслеживанию
* Git version - просматриваем установленную версию
 
~~Тильда~~

***git status***
 
* Git log - выводится вся информация о commite
* Git checkout - возвращает к commity
* Git checkout master - возвращает к актуальной версии
* git diff - разность между файлами
 
* изменения после лекции

 1 изменения после ужина
 
 2 изменения после борьбы с компьютером
 
3 изменения после новых непоняток 

4 опять непонятно

* git diff (commit 1 - commit 2 --- 5-7 символов)

 ## Ссылки

 ## Работа с таблицами

 ## Цитаты

 ## Заключения


 Домашнее задание


   # Семинар 2 #

__создание новых веток__

Команда git brench "name" - создание новой ветки

Команда git branch - проверку созданных веток

__слияние веток__

Команда git merge "name" проиводит слияние веток


__конфликт при слиянии веток__

при конфликте веток в ручную выбирается способ решения конфликта
Git branch konflict2

 * Лекция №2
тоесть не 2, а 3!!

1. Cоздали аккаунт на GITHUB
2. Создали локальный репозиторий
3. Подружить локальный и удаленный репозиторий
4. Отправили (PUSH) локальный в удаленный
5. Провели изменения на GiTHUB
6. Выкачать (Pull) актуальное состояние из удаленного
  Пытаемся организовать
  конфликт сделав комментарии в общем пространстве

December2022
 
 * Семинар №3 DZ

# Клонирование репозитория

git clone git@github.com:nicothin/web-design.git # клонировать удаленный репозиторий в одноименную папку
git clone git@github.com:nicothin/web-design.git foldername # клонировать удаленный репозиторий в папку «foldername»
git clone git@github.com:nicothin/web-design.git . # клонировать репозиторий в текущую папку

# Удалённые репозитории

git remote -v # показать список удалённых репозиториев, связанных с этим
git remote remove origin # убрать привязку удалённого репозитория с сокр. именем origin
git remote add origin git@github.com:nicothin/test.git # добавить удалённый репозиторий (с сокр. именем origin) с указанным URL
git remote rm origin # удалить привязку удалённого репозитория
git remote show origin # получить данные об удалённом репозитории с сокращенным именем origin
git fetch origin # скачать все ветки с удаленного репозитория (с сокр. именем origin), но не сливать со своими ветками
git fetch origin master # то же, но скачивается только указанная ветка
git checkout origin/github_branch # посмотреть ветку, скачанную с удалённого репозитория (локальной редактируемой копии не создаётся! если нужно редактировать, придётся влить)
git checkout --track origin/github_branch # создать локальную ветку github_branch (данные взять из удалённого репозитория с сокр. именем origin, ветка github_branch) и переключиться на неё
git push origin master # отправить в удалённый репозиторий (с сокр. именем origin) данные своей ветки master
git pull origin # влить изменения с удалённого репозитория (все ветки)
git pull origin master # влить изменения с удалённого репозитория (только указанная ветка)

# Начало работы

# указана последовательность действий:
git init # инициируем гит в этой папке
touch readme.md # создаем файл readme.md
git add readme.md # делаем этот файл отслеживаемым
git commit -m "Первый коммит" # создаем первый коммит с вменяемым названием
git remote add origin git@github.com:nicothin/test.git # добавляем предварительно созданный пустой удаленный репозиторий
git push origin master # отправляем данные из локального репозитория в удаленный (в ветку master)
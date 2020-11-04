# Git консольные команды

git init - инициализируем git

git status - статус git'а

git add . - добавить все папки в отслеживаение git

git commit -m "" - добавить коммит с сообщением

git branch -M main - переименовываем ветку master в main

git remote add origin url - подключаем git к удаленому репозиторию

git remote add pb url - подключаемся к удаленому репозиторию

git push -u origin main - загружаем на Github ветку main

git push - загрузить на Github

git pull - скачать с Github

# Git последовательность дейстивий при подключении к пустому репозиторию

git init

git add .

git commit -m "Сообщение"

git branch -M main

git remote add origin url

git push -u origin main

# Git последовательность дейстивий при подключении к рабочему репозиторию

Зайти папку, в которой будет располагаться скаченный репозиторий с Github

git clone url

Зайти в саму папку, скаченного репозитория (cd папка)

git remote add pb url

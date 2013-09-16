MyRepository
============
Мой маленький мануальчик =)

// Как создать свой репозиторий на GitHub //
mkdir MyRepository // Создание папки с именем MyRepository
cd MyRepository // Переход к папке MyRepository
touch FileName // Создание файла с именем FileName
git init // Создание пустого локального репозитория
git add . // Добавление всех файлов в режим ожидания
git add FileName // Добавление файла FileName в режим ожидания
git commit -m 'Firts Commit' // Первый коммит (фиксация изменений)
git commit -a //Совершит коммит, автоматически индексируя изменения в файлах проекта.
git remote add server https://github.com/DoSyMeP/MyRepository.git // Добавление серверного репозитория с именем server
git push server master:master / /Отправление данных репозитория с именем server на удаленный сервер
git pull https://github.com/DoSyMeP/MyRepository // Обновление локального репозитория из удаленного
git pull server master // Обновление локального репозитория из удаленного укороченная версия
Создание репозитория с именем MyRepository

master // Ветка репозитория

git remote rename server MyRepository // Переименовывает ссылку репозитория server в MyRepository

git remote rm server / /Удаление ссылки репозитория с именем server
git rm FILE1 FILE2 // Отдельные файлы
git rm Documentation/\*.txt // Удаления сразу всех файлов txt из папки.

git status // Состояние проекта
git remote 
git remote -v


git log // Просмотр истории коммитов

$ git commit -m 'initial commit'
$ git add forgotten_file
$ git commit --amend // Когда сделали коммит раньше чем добавили шунжный файл

git branch -d master // Удаление ветки master
git checkout features // Создание ветки features или переход на ветку ftanures

git tag // Тэги как способ пометить уникальный коммит

// Как внести изменения в чужой проект //
git clone https://github.com/reenboog/omgupsLectures // Создания клона репозитория omgupsLectures c именем omgupsLectures
// Eсли хотите поменять имя репозитория то его надо дописать в конце
cd omgupsLectures // Перейти в папку omgupsLectures
git remote add upstream https://github.com/reenboog/omgupsLectures // Создание привязки отслеживающие изменения в данном репозитории
git fetch upstream // Обновление upstream
git checkout -b feature // Создаёт новую ветвь, названную "feature" и делает её активной
git push origin feature // Загружает изменения в текущей ветви в origin в ветвь feature
// Когда ваш pull request примут, не забудьте слить изменения в свой репозиторий (или удалить его, если больше не нужен) //
git checkout master
git pull upstream master
git push origin master
// Так же можно удалить ветку, в которой велась разработка //
git branch -d feature // В локальном репозитории
git push origin :feature // В удалённом репозитории

// Как внести изменения в чужой проект //
http://habrahabr.ru/post/125999/

// Основные команды GitHub, без которых сложно жить с GitHub'ом //
http://habrahabr.ru/post/60347/

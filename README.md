Мой маленький мануальчик =)
============

Как создать свой репозиторий на GitHub
-------------------------

mkdir MyRepository // Создание папки с именем MyRepository <br/>
cd MyRepository // Переход к папке MyRepository <br/>
touch FileName // Создание файла с именем FileName <br/>
git init // Создание пустого локального репозитория <br/>
git add . // Добавление всех файлов в режим ожидания <br/>
git add FileName // Добавление файла FileName в режим ожидания <br/>
git commit -m 'Firts Commit' // Первый коммит (фиксация изменений) <br/>
git commit -a //Совершит коммит, автоматически индексируя изменения в файлах проекта. <br/>
git remote add server https://github.com/DoSyMeP/MyRepository.git // Добавление серверного репозитория с именем server <br/>
git push server master:master / /Отправление данных репозитория с именем server на удаленный сервер <br/>
git pull https://github.com/DoSyMeP/MyRepository // Обновление локального репозитория из удаленного <br/>
git pull server master // Обновление локального репозитория из удаленного укороченная версия <br/>

Как внести изменения в чужой проект
-------------------------

git clone https://github.com/reenboog/omgupsLectures // Создания клона репозитория omgupsLectures c именем omgupsLectures
// Eсли хотите поменять имя репозитория то его надо дописать в конце <br/>
cd omgupsLectures // Перейти в папку omgupsLectures <br/>
git remote add upstream https://github.com/reenboog/omgupsLectures // Создание привязки отслеживающие изменения в данном репозитории <br/>
git fetch upstream // Обновление upstream <br/>
git checkout -b feature // Создаёт новую ветвь, названную "feature" и делает её активной <br/>
git push origin feature // Загружает изменения в текущей ветви в origin в ветвь feature <br/>
###### Когда ваш pull request примут, не забудьте слить изменения в свой репозиторий (или удалить его, если не нужен) ######
> git checkout master <br/>
> git pull upstream master <br/>
> git push origin master <br/>

Вспомогательные команды
-------------------------
git remote rename server MyRepository // Переименовывает ссылку репозитория server в MyRepository <br/>
git remote rm server / /Удаление ссылки репозитория с именем server <br/>
git rm FILE1 FILE2 // Отдельные файлы <br/>
git rm Documentation/\*.txt // Удаления сразу всех файлов txt из папки. <br/>
git status // Состояние проекта <br/>
git remote 
git remote -v
git log // Просмотр истории коммитов <br/>
git tag // Тэги как способ пометить уникальный коммит <br/>

###### Когда сделали коммит раньше чем добавили нужный файл ######
-------------------------

> git commit -m 'initial commit' <br/>
> git add forgotten_file <br/>
> git commit --amend<br/>

Ветки
-------------------------

git branch -d master // Удаление ветки master <br/>
git checkout features // Создание ветки features или переход на ветку features <br/>
###### Так же можно удалить ветку, в которой велась разработка ######
> git branch -d feature // В локальном репозитории <br/>
> git push origin :feature // В удалённом репозитории <br/>

Сыллки
-------------------------

Книжка про GitHub <br/>
http://git-scm.com/book/ru <br/>

// Как внести изменения в чужой проект // <br/>
http://habrahabr.ru/post/125999/ <br/>

// Основные команды GitHub, без которых сложно жить с GitHub'ом // <br/>
http://habrahabr.ru/post/60347/ <br/>

// Синтаксис файла README.md // <br/>
https://github.com/OlgaVlasova/markdown-doc/blob/master/README.md <br/>

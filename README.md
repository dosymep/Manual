MyRepository
============

Final Test

Мой маленький мануальчик =)

mkdir MyRepository //Создание папки с именем MyRepository 
cd MyRepository //Переход к папке MyRepository 
touch FileName //Создание файла с именем FileName 
git init //Создание пустого локального репозитория
git add FileName //Добавление файла FileName в локальный репозиторий
git commit -m 'Firts Commit' //Первый коммит (фиксация изменений)
git commit -a //Совершит коммит, автоматически индексируя изменения в файлах проекта.
git remote add server https://github.com/DoSyMeP/MyRepository.git //Добавление серверного репозитория с именем server
git push server master:master //Отправление данных репозитория с именем server на удаленный сервер
git pull https://github.com/DoSyMeP/MyRepository //Обновление локального репозитория из удаленного
git pull server master //Обновление локального репозитория из удаленного укороченная версия
Создание репозитория с именем MyRepository

master //ветка репозитория

git remote rename server MyRepository //Переименовывает ссылку репозитория server в MyRepository

git remote rm server //Удаление ссылки репозитория с именем server
git rm FILE1 FILE2 //Отдельные файлы
git rm Documentation/\*.txt //Удаления сразу всех файлов txt из папки.

git status //Состояние проекта

git remote 

git remote -v

git clone https://github.com/reenboog/omgupsLectures //Создания клона репозитория omgupsLectures c именем omgupsLectures, если хотите поменять имя репозитория то его надо дописать в конце

git log //Просмотр истории коммитов подробней про параметров команды http://git-scm.com/book/ru/%D0%9E%D1%81%D0%BD%D0%BE%D0%B2%D1%8B-Git-%D0%9F%D1%80%D0%BE%D1%81%D0%BC%D0%BE%D1%82%D1%80-%D0%B8%D1%81%D1%82%D0%BE%D1%80%D0%B8%D0%B8-%D0%BA%D0%BE%D0%BC%D0%BC%D0%B8%D1%82%D0%BE%D0%B2

$ git commit -m 'initial commit' 
$ git add forgotten_file
$ git commit --amend //Когда сделали коммит раньше чем добавили шунжный файл

С ветками еще не разобрался

git add . //Добавление файлов в режим ожидания

git branch -d master //Удаление ветки master

git tag //Тэги как способ пометить уникальный коммит

http://habrahabr.ru/post/60347/

Основные команды GitHub, без которых сложно жить с GitHub'ом

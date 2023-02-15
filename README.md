В проекте применены
Сборка docker образов для работы: nginx, django + gunicorn, postgres. Проброшены на локальный хост папки для дальнейшей разработки проекта (django, static, media). Файлы базы данных postgres так же сохраняются на хосте (папка postgres) для сохранения внесенных изменений в случае перезапуска контейнеров.

Установка docker
Для lunix систем:
curl -fsSL https://get.docker.com/ | sh //Установка Docker
Для Windows или Macos:
https://www.docker.com/ //Установка Docker Desktop

Запуск приложения:
После установки docker, загружаем проект командой:
git clone https://github.com/PIvanV/Modul_G4.git
В командной строке, переходим в директорию проекта и набираем:
sudo docker-compose up -d //В среде lunix docker-compose up -d //Docker Desktop (Windows или Macos) После завершения установки и запуска контейнеров, заходим в браузере по адресу:
(в случае не запуска какого-либо контейнера, запустить его в ручную) http://localhost:1337
Войти на страницу администрирования можно по адресу:
http://localhost:1337/admin
логин: admin
пароль: admin

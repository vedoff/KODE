# KODE
## Тестовое задание
1. Создать репозиторий Ansible и написать роли
 - Обновить систему (Debian, CentOS)
 - установить пакеты curl, wget, htop
 - создать двух пользователей
 - добавить пользователей в суперюзеры
2. Создать репозиторий Docker в нем создать Dockerfile. \
   В файле необходимо обновить систему и создать задание для крона, которое будет раз в час
   добавлять 1 в файл test.log
### Тестировал с использованием Vagrant оставил полный вариант.
## №1
`cd Ansible && ansible-playbook play.yml --ask-vault-pass`\
`vault-pass = 123456`\
Пароли на пользователей `123456`
## №2
Можно запустить при помощи Vagrant или скопировать содержимое папки provision на хост \
запустить скрипт установки docker docker-compose и выполнить \
`docker-compose up -d` 

[Ссылка на референс](https://ivan.bessarabov.ru/blog/how-to-run-cron-in-docker)

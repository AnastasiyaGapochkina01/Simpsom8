1) Написать плейбук по установке apache. Плейбук должен учитывать, что на целевых хостах может быть как debian, так и centos (redhat)
2) Написать роли для установки
- nginx. Роль должна включать создание конфигурационного файла сайта из шаблона, в котором переменными будут например доменное имя и папка проекта
- php (php-fpm). Роль должна включать настройку timezone
- mariadb-server. Роль должна включать создание нового админского пользователя и установку ему пароля
3) Написать роль для установки node-exporter (НЕ в docker)
4) Написать роль, которая настроит replicaset mongodb
5) Написать роль для установки и конифгурации iptables
- роль должна включать в себя возможность добавить/удалить правило на целевом хосте
6) Написать роль для раскатки приложения https://github.com/AnastasiyaGapochkina01/linux_app

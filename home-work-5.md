1) Написать скрипт, который будет проверять состояние указанных служб и перезапускать их, если они остановлены. (названия можно захардкодить к скрипте, а не передавать аргементом)
2) Написать скрипт для поиска свободных портов из диапазона 12450-12462
3) Написать скрипт для сбора статистики о процессах:
- об использовании cpu
- об использовании памяти
- выводить парамтеры pid, user, command и cpu/mem
- выводить только первые 5 процессов в списке, отсортированных по нужному параметру
- результат должен записываться в файл /var/log/process_stat.log в формате
```
==> Process stats at 2024-24-10_12-11-35 <==
--------------------------------------------
==> CPU usage <==
%CPU     PID USER     COMMAND
15.8     517 jenkins  /usr/bin/java -Djava.awt.headless=true -jar /usr/share/java/jenkins.war --webroot=/var/cache/jenkins/war --httpPort=8080
 3.8       1 root     /sbin/init
 1.6     554 root     /sbin/agetty -o -p -- \u --keep-baud 115200,57600,38400,9600 ttyS0 vt220
 0.9     270 root     /lib/systemd/systemd-udevd
==> MEM usage <==
SIZE     PID USER     COMMAND
797876    517 jenkins  /usr/bin/java -Djava.awt.headless=true -jar /usr/share/java/jenkins.war --webroot=/var/cache/jenkins/war --httpPort=8080
26044     431 root     /sbin/dhclient -4 -v -i -pf /run/dhclient.eth0.pid -lf /var/lib/dhcp/dhclient.eth0.leases -I -df /var/lib/dhcp/dhclient6.eth0.leases eth0
26044     458 root     /sbin/dhclient -4 -v -i -pf /run/dhclient.eth0.pid -lf /var/lib/dhcp/dhclient.eth0.leases -I -df /var/lib/dhcp/dhclient6.eth0.leases eth0
18636     519 root     /usr/sbin/rsyslogd -n -iNONE
```
4) Написать скрипт для автоматической установки nginx+php-fpm+percona. Скрипт должен проверять, установилось ли ПО запросом версии и выводить отчет об установленных версиях в файл output.txt
5) Написать скрипт, который будет получать сколько процентов диска использовано (команда ```df```) и делать запись в файл /var/log/disk_space.log, если это число превысило 80%
6) Написать скрипт, который автоматизирует создание пользователей:
- имя пользователя передается скрипту как аргумент
- при создании пользователя обязательно создать ему домашнюю директорию и установить интерпретатор /bin/bash
- сгененрировать пароль и установить его пользователяю
- сделать заготовку под отправку e-mail пользователю о том, что ему создали учетную запись (заготовку, тк почта ходить скорее всего не будет)

# Часть 1
1) В домашнем каталоге создать директорию lab_1
2) В lab_1 создать директорию storage
3) В директории storage создать каталог foodstuff
4) В директории storage создать каталог household_chemicals
5) В директории storage создать каталог toys
6) Перейти в каталог foodstuff
7) Создать в foodstuff директории fruits, groceries, milk_products
8) Не выходя из foodstuff содать в storage/household_chemicals директории cosmetic, laundry_products, cleaning_products
9) Не выходя из foodstuff содать в storage/toys директории educational_toys, soft_toys
10) Перейти в каталог foodstuff
11) В директории storage/foodstuff/fruits создать файл с именем apples и содержимым
```
Golden
Gala
Caramel
Fuji
Red
```
12) В директории storage/household_chemicals/cleaning_products создать файл с именем floor_products и содержимым
```
Mr Proper
Grass
Synergetic
```
13) В директории storage/household_chemicals/laundry_products создать файл с именем powders и содержимым
```
Persil
Laska
Tide
Ariel
```
14) Перейти в директорию storage/household_chemicals/cleaning_products
15) Не выходя из storage/household_chemicals/cleaning_products создать в storage/household_chemicals/cosmetic файл с именем lipsticks и содержимым
```
Beloris
Luxvisage
Novo Small
```
16) Не выходя из storage/household_chemicals/cleaning_products создать в storage/toys/educational_toys файл с именем constructors и содержимым
```
Arduino
Lego
```
17) Не выходя из storage/household_chemicals/cleaning_products создать в storage/toys/soft_toys файл с именем all_products и содержимым
```
Bear
Gouse
Lion
Tiger
```
18) Перейти в директорию storage/toys/soft_toys
19) Не выходя из storage/toys/soft_toys скопировать файл с именем all_products в storage/toys/
20) Не выходя из storage/toys/soft_toys создать РЯДОМ с директорией storage директорию shipment
21) Не выходя из storage/toys/soft_toys скопировать файл storage/foodstuff/fruits/apples в директорию shipment
22) Не выходя из storage/toys/soft_toys скопировать файл storage/household_chemicals/cleaning_products/floor_products в директорию shipment
23) Скопировать директорию storage/toys/ в директорию shipment
24) Скопировать содержимое storage/household_chemicals/ в директорию shipment
25) Выполнить команды tree -a shipment и tree -a storage
# Часть 2
1) Получить информацию о HugePages из файла /proc/meminfo. (Там скорее всего будет по нулям и это норма)
2) Получить информацию о количестве ядер cpu из файла /proc/cpuinfo (строка cpu cores)
3) Получить id (3 поле в строке) пользователя www-data офильтровав содержимое файла /etc/passwd
4) Создать в директории inform_фамилия папку text_processing
5) Создать файл info.csv с таким содержимым
```
Name,Company,Price,Ganre,Multiplayer
Item1,Company1,60000$,Ganre1,Yes
Item2,Company2,70000$,Ganre2,Yes
Item3,Company3,90000$,Ganre1,Yes
Item4,Company4,90000$,Ganre1,Yes
Item5,Company5,110000$,Ganre1,Yes
Item6,Company6,410000$,Ganre2,Yes
```
6) Вывести первые две строки файла info.csv
7) Вывести стобец Price
8) Найти все строки, в которых встречается слово Ganre2
9) Найти все строки, в которых встречается слово Ganre2 и вывести для них столбец Price
10) Дозаписать в файл info.csv с помощью echo строку Item7,Company6,450000\$,Ganre1,No
11) Получить из файла /proc/cpuinfo model name
12) Создать файл inventory с содержимым
```
[Compute1]
IP_Address = 192.168.1.100
Location = Datacenter A
Service_Name = Web Server

[Compute2]
IP_Address = 192.168.1.101
Location = Datacenter B
Service_Name = Database Server

[Compute3]
IP_Address = 192.168.1.102
Location = Datacenter C
Service_Name = Application Server

[Compute4]
IP_Address = 192.168.1.103
Location = Datacenter A
Service_Name = File Server

[Compute5]
IP_Address = 192.168.1.104
Location = Datacenter B
Service_Name = Mail Server
```
13) С помощью grep в файле inventory найти все хосты, которые относятся к Datacenter B
14) С помощью grep в файле inventory найти все хосты, которые относятся к Datacenter C и вывести только их ip
15) Отфильровать вывод команды lscpu так, чтобы получить значение CPU MHz
16) Отфильровать вывод команды lscpu так, чтобы получить значение Hypervisor vendor
17) Отфильтровать вывод команды lsblk так, чтобы получить все разделы (раздел это та строка, где 6 поле имеет значение part)
18) Для полученных в предыдущем задании разделов вывести их имена
19) С помощью awk вывести из файла /etc/passwd имена всех пользователей (первое поле)
20) С помощью awk вывести из файла /etc/passwd последнее поле
21) Отфильтровать вывод команды free -h так, чтобы получить размер Swap

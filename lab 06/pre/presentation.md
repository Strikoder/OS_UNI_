---
## Front matter
lang: ru-RU
title: lab 6
author: |
	Mohamad alamin Yassin
institute: |
	\inst{1}RUDN University, Moscow, Russian Federation
	

## Formatting
toc: false
slide_level: 2
theme: metropolis
header-includes: 
 - \metroset{progressbar=frametitle,sectionpage=progressbar,numbering=fraction}
 - '\makeatletter'
 - '\beamer@ignorenonframefalse'
 - '\makeatother'
aspectratio: 43
section-titles: true
---
# Презентация к лабораторной работе №6

# Анализ файловой системы Linux. Команды для работы с файлами и каталогами

----

## Российский Университет Дружбы Народов

### Факультет Физико-Математических и Естественных Наук

*Дисциплина: Операционные системы*

Студент: Яссин мохамад аламин

Группа: нкн-01-20

Москва, 2021г.

----

### Цель работы

Ознакомление с файловой системой Linux, её структурой, именами и содержанием каталогов. Приобретение практических навыков по применению команд для работы с файлами и каталогами, по управлению процессами (и работами), по проверке использования диска и обслуживанию файловой системы.

### Ход работы:
1. Выполнил все примеры, приведённые в первой части описания лабораторной работы.
![](https://github.com/Strikoder/OS/blob/main/lab%2006/report/img/6.1.JPG?raw=true)
![](https://github.com/Strikoder/OS/blob/main/lab%2006/report/img/6.3.JPG?raw=true)
2.	Выполнил следующие действия:

* Скопировал файл /usr/include/sys/io.txt в домашний каталог и назвал его equipment.
* В домашнем каталоге создал директорию ~/ski.plases.
* Переместил файл equipment в каталог ~/ski.plases.
* Переименовал файл ~/ski.plases/equipment в ~/ski.plases/equiplist.
*  домашнем каталоге создал файл abc1 и скопировал его в каталог ~/ski.plases, назвал его equiplist2.
* Создал каталог с именем equipment в каталоге ~/ski.plases.
* Переместил файлы ~/ski.plases/equiplist и equiplist2 в каталог ~/ski.plases/equipment.
* Создал и переместил каталог ~/newdir в каталог ~/ski.plases, назвав его plans.
  
3.	Определил опции команды chmod, необходимые для того, чтобы присвоить перечисленным ниже файлам выделенные права доступа, считая, что в начале таких прав нет:

* drwxr--r-- ... australia
* drwx--x--x ... play
* -r-xr--r-- ... my_os
* -rw-rw-r-- ... feathers
![](https://github.com/Strikoder/OS/blob/main/lab%2006/report/img/6.10.JPG?raw=true)
4.	Проделал приведённые ниже упражнения, записывая в отчёт по лабораторной работе используемые при этом команды:

* Просмотрел содержимое файла /etc/password.
![](https://github.com/Strikoder/OS/blob/main/lab%2006/report/img/6.11.JPG?raw=true)



---
  
  ### Вывод

Ознакомился с файловой системой Linux, её структурой, именами и содержанием каталогов. Приобрел практические навыки по применению команд для работы с файлами и каталогами, по управлению процессами (и работами), по про- верке использования диска и обслуживанию файловой системы.

----
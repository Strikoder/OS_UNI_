---
# Front matter
lang: ru-RU
title: "Шаблон отчёта по 1 лабораторной работе"
subtitle: "Простейший вариант"
author: "Яссин мохамад аламин"

# Formatting
toc-title: "Содержание"
toc: true # Table of contents
toc_depth: 2
lof: true # List of figures
lot: true # List of tables
fontsize: 12pt
linestretch: 1.5
papersize: a4paper
documentclass: scrreprt
polyglossia-lang: russian
polyglossia-otherlangs: english
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase
indent: true
pdf-engine: lualatex
header-includes:
  - \linepenalty=10 # the penalty added to the badness of each line within a paragraph (no associated penalty node) Increasing the value makes tex try to have fewer lines in the paragraph.
  - \interlinepenalty=0 # value of the penalty (node) added after each line of a paragraph.
  - \hyphenpenalty=50 # the penalty for line breaking at an automatically inserted hyphen
  - \exhyphenpenalty=50 # the penalty for line breaking at an explicit hyphen
  - \binoppenalty=700 # the penalty for breaking a line at a binary operator
  - \relpenalty=500 # the penalty for breaking a line at a relation
  - \clubpenalty=150 # extra penalty for breaking after first line of a paragraph
  - \widowpenalty=150 # extra penalty for breaking before last line of a paragraph
  - \displaywidowpenalty=50 # extra penalty for breaking before last line before a display math
  - \brokenpenalty=100 # extra penalty for page breaking after a hyphenated line
  - \predisplaypenalty=10000 # penalty for breaking before a display
  - \postdisplaypenalty=0 # penalty for breaking after a display
  - \floatingpenalty = 20000 # penalty for splitting an insertion (can only be split footnote in standard LaTeX)
  - \raggedbottom # or \flushbottom
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

#Отчёт о выполнении лабораторной работы №1 
---

# Цель работы

Целью данной работы является приобретение навыков установки системы CentOS на виртуальную машину с настройками

# Задание

Скачать VirtualBox и установить на него centos


# Выполнение лабораторной работы

1. Я установил на мой ПК Oracle Virtual Machine (рис. -@fig:001) 
![Oracle VM](img/1.1.jpg) { #fig:001 width=70% }
2. Настраиваю VM для установки Linux CentOS  
	- Указываю имя виртуальной машины и тип гостевой ОС  
	![Имя ВМ и тип ОС](img/1.2.jpg)
	- Выделяю для работы ~7000 Мб оперативной памяти  
	![Оперативная память](img/1.3.jpg)
	- Создаю виртуальный диск типа VDI объемом 20 Гб  
	![Выбор типа диска](img/1.4.jpg)
	
	![Подключение образа](img/1.5.jpg)
3. Пошаговая установка и настройка CentOS  
	- В разделе "Выбор приложений" выбираем "Сервер с GUI"  
	![Выбор приложений](img/1.6.jpg)
	- включим сить
	![включим сить](img/1.7.jpg)
	- Отключаю KDUMP  
	![Отключение KDUMP]()
	- Ожидаю окончания установки  
	![Установка](image/3.4.png)
	- Принимаем лицензионное соглашение  
	![Лицензионное соглашение](image/3.5.png)
4. Подключаю образ диска дополнений гостевой ОС  
![Установка образа](image/4.1.png)

# Домашнее задание

1. Анализирую последовательность загрузки системы с помощью команды ```dmesg | less```  
![dmesg в терминале](image/hw1.png)
2. Получаем необходимую информацию с помощью команды ```dmesg | grep -i "..."```  
    1. Версия ядра линукс  
    ![Linux Version](image/hw2.png)
    2. Частота процессора  
    ![Частота процессора](image/hw3.png)
    3. Модель процессора  
    ![Модель процессора](image/hw4.png)
    4. Объем доступной оперативной памяти  
    ![Объем доступной оперативной памяти](image/hw5.png)
    5. Тип обнаруженного гипервизора  
    ![Тип обнаруженного гипервизора](image/hw6.png)
    6. Тип файловой системы корневого раздела  
    ![Тип файловой системы корневого раздела](image/hw7.png)
    7. Последовательность монтирования файловых систем  
    ![Последовательность монтирования файловых систем](image/hw8.png)

# Выводы

Данная лабораторная работа помогла мне научиться устанавливать и использовать виртуальную машину для работы.
Я научился производить первоначальную настройку Oracle VM для работы с ОС CentOS.
Также я научился использовать команду ```dmesg``` для поиска нужной информации о системе.

# Контрольные вопросы

1. Учетная запись пользователя содержит такие команды, как:
	- Системное имя пользователя
	- Пароль
	- Уникальный идентификатор пользователя (UID)
	- Идентификатор группы пользователя (GID)
	- Директория, в которой работает пользователь

2. Команды терминала:
	1. Для получения справки по команде используется флаг ```--help``` или ```-h```, 
	например ```cd --help```
	2. Для перемещения по файловой системе используется команда ```cd```,
	например 
	```cd downloads``` - перемещение в каталог "downloads" 
	```cd ..``` - перемещение в корневой каталог
	3. Для просмотра содержимого каталога используется команда ```ls```
	4. Для определения объема каталога используется команда ```du```
	Для удобства лучше использовать с ключами ```-s``` и ```-h```
	например ```du -hs /downloads```
	5. Чтобы создать файл или каталог, используются команды ```touch``` и ```mkdir``` соответственно
	например ```touch text.txt```, ```mkdir downloads2```
	Чтобы удалить файл или каталог, используются команды ```rm``` и ```rmdir``` соответственно
	например ```rm text.txt```, ```rmdir downloads2```
	6. Для создания и редактирования прав файла/каталога используют ```chmod```
	например ```chmod 777 text.txt```
	7. Для просмотра истории команд используют  ```history```
3. Файловая система - это порядок, определяющий организацию, структуру, хранение и именование на определенном логическом носителе
Примеры наиболее распространенных файловых систем: *NTFS*, *FAT32*, *exFAT*
4. Узнать, какие ФС смонтированы в ОС, можно узнать с помощью команды ```mount```
5. Можно использовать команду ```killall *Process Name*```

















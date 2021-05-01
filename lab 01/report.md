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
  * \linepenalty=10 # the penalty added to the badness of each line within a paragraph (no associated penalty node) Increasing the value makes tex try to have fewer lines in the paragraph.
  * \interlinepenalty=0 # value of the penalty (node) added after each line of a paragraph.
  * \hyphenpenalty=50 # the penalty for line breaking at an automatically inserted hyphen
  * \exhyphenpenalty=50 # the penalty for line breaking at an explicit hyphen
  * \binoppenalty=700 # the penalty for breaking a line at a binary operator
  * \relpenalty=500 # the penalty for breaking a line at a relation
  * \clubpenalty=150 # extra penalty for breaking after first line of a paragraph
  * \widowpenalty=150 # extra penalty for breaking before last line of a paragraph
  * \displaywidowpenalty=50 # extra penalty for breaking before last line before a display math
  * \brokenpenalty=100 # extra penalty for page breaking after a hyphenated line
  * \predisplaypenalty=10000 # penalty for breaking before a display
  * \postdisplaypenalty=0 # penalty for breaking after a display
  * \floatingpenalty = 20000 # penalty for splitting an insertion (can only be split footnote in standard LaTeX)
  * \raggedbottom # or \flushbottom
  * \usepackage{float} # keep figures where there are in the text
  * \floatplacement{figure}{H} # keep figures where there are in the text
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
	*Указываю имя виртуальной машины и тип гостевой ОС  
	![Имя ВМ и тип ОС](img/1.2.jpg)
	* Выделяю для работы ~7000 Мб оперативной памяти  
	![Оперативная память](img/1.3.jpg)
	* Создаю виртуальный диск типа VDI объемом 20 Гб  
	![Выбор типа диска](img/1.4.jpg)
	
	![Подключение образа](img/1.5.jpg)
3. Пошаговая установка и настройка CentOS  
	* В разделе "Выбор приложений" выбираем "Сервер с GUI"  
	![Выбор приложений](img/1.6.jpg)
	* включим сить
	![включим сить](img/1.7.jpg)
	* Username+password  
	![Установка](img/1.8.jpg)
4. Всё работает хорошо
![Установка образа](img/1.9.jpg)

# Домашнее задание

1. Анализирую последовательность загрузки системы с помощью команды dmesg | less  
![dmesg в терминале](image/hw1.png)
2. Получаем необходимую информацию с помощью команды dmesg | grep -i "..."  
    1. Linux's version 
    ![Linux's Version](img/2.jpg)
    1. CPU 
    ![Частота процессора](img/3.jpg)
    1. CPU Model
    ![Модель процессора](img/4.jpg)
    1. Size of memory 
    ![Объем доступной оперативной памяти](img/5.jpg)
    1. Hypervisor vendor
    ![Тип обнаруженного гипервизора](img/6.jpg)
    1. The file system type of the root partition 
    ![Тип файловой системы корневого раздела](img/7.jpg)
    1. Sequence of mounting filesystems
    ![Последовательность монтирования файловых систем](img/8.jpg)



# Контрольные вопросы

1. Учетная запись пользователя содержит такие команды, как:
	* Системное имя пользователя
	* Пароль
	* Уникальный идентификатор пользователя (UID)
	* Идентификатор группы пользователя (GID)
	* Директория, в которой работает пользователь

2. Команды терминала:
	1. Для получения справки по команде используется флаг --help или -h, 
	например cd --help
	2. Для перемещения по файловой системе используется команда cd,
	например 
	cd downloads * перемещение в каталог "downloads" 
	cd .. * перемещение в корневой каталог
	3. Для просмотра содержимого каталога используется команда ls
	4. Для определения объема каталога используется команда du
	Для удобства лучше использовать с ключами -s и -h
	например du -hs /downloads
	5. Чтобы создать файл или каталог, используются команды touch и mkdir соответственно
	например touch text.txt, mkdir downloads2
	Чтобы удалить файл или каталог, используются команды rm и rmdir соответственно
	например rm text.txt, rmdir downloads2
	6. Для создания и редактирования прав файла/каталога используют chmod
	например chmod 777 text.txt
	7. Для просмотра истории команд используют  history
3. Файловая система * это порядок, определяющий организацию, структуру, хранение и именование на определенном логическом носителе
Примеры наиболее распространенных файловых систем: *NTFS*, *FAT32*, *exFAT*
4. Узнать, какие ФС смонтированы в ОС, можно узнать с помощью команды mount
5. Можно использовать команду killall *Process Name*


# Вывод
Эта лабораторная работа помогла мне узнать, как настроить и использовать виртуальную машину для работы.
Я узнал, как выполнить первоначальную настройку виртуальной машины OracleVM для работы с ОС CentOS.
Я также научился использовать команду dmesg и некоторые другие команды для поиска необходимой системной информации.












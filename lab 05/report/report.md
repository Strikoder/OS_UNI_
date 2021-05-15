---
# Front matter
lang: ru-RU
title: "lab 05"
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




# Отчёт о выполнении лабораторной работы №5 
***Российский Университет Дружбы Народов***  
***Факульткт Физико-Математических и Естественных Наук***  

 ***Дисциплина:*** *Операционные системы*  
 
 ***Работу выполняла:*** Яссин мохамад аламин 
 
 
 *НКНбд-01-20*  
 
 ***Москва РУДН. 2021г.***  
 

# Цель работы

Приобретение практических навыков взаимодействия пользователя с системой
посредством командной строки.

# Задание

1. Определите полное имя вашего домашнего каталога. Далее относительно этого каталога будут выполняться последующие упражнения.
2. Выполните следующие действия:
2.1. Перейдите в каталог /tmp .
2.2. Выведите на экран содержимое каталога /tmp . Для этого используйте команду ls с различными опциями. Поясните разницу в выводимой на экран
информации.
2.3. Определите, есть ли в каталоге /var/spool подкаталог с именем cron ?
2.4. Перейдите в Ваш домашний каталог и выведите на экран его содержимое.
Определите, кто является владельцем файлов и подкаталогов?
3. Выполните следующие действия:
3.1. В домашнем каталоге создайте новый каталог с именем newdir .
3.2. В каталоге ~/newdir создайте новый каталог с именем morefun .
3.3. В домашнем каталоге создайте одной командой три новых каталога с именами letters , memos , misk . Затем удалите эти каталоги одной командой.
3.4. Попробуйте удалить ранее созданный каталог ~/newdir командой rm . Проверьте, был ли каталог удалён.
3.5. Удалите каталог ~/newdir/morefun из домашнего каталога. Проверьте, был ли каталог удалён.
4. С помощью команды man определите, какую опцию команды ls нужно использовать для просмотра содержимое не только указанного каталога, но и подкаталогов, входящих в него.
5. С помощью команды man определите набор опций команды ls , позволяющий отсортировать по времени последнего изменения выводимый список содержимого каталога с развёрнутым описанием файлов.
6. Используйте команду man для просмотра описания следующих команд: cd , pwd , mkdir , rmdir , rm . Поясните основные опции этих команд.
7. Используя информацию, полученную при помощи команды history , выполните модификацию и исполнение нескольких команд из буфера команд.

# Выполнение лабораторной работы

1. Имя моего каталога с помощью команды *pwd* (рис. -@fig:001)

![Имя каталога](https://github.com/Strikoder/OS/blob/main/lab%2005/report/img/5.1.JPG?raw=true) { #fig:001 width=70% }

1. Выполнил следующие действия:

2.1 Перешел в /tmp и вывел на экран содержимое каталога /tmp.
- с командой -ls (рис. -@fig:002)

![Команда ls](https://github.com/Strikoder/OS/blob/main/lab%2005/report/img/5.2.JPG?raw=true) { #fig:002 width=70% }

- с командой -ls -a (рис. -@fig:003)

![Команда ls -a](https://github.com/Strikoder/OS/blob/main/lab%2005/report/img/5.3.JPG?raw=true) { #fig:003 width=70% }

- с командой -ls -l (рис. -@fig:004)

![Команда ls -l](https://github.com/Strikoder/OS/blob/main/lab%2005/report/img/5.4.JPG?raw=true) { #fig:004 width=70% }

2.2 Да, в каталоге /var/spool есть подкаталог с именем cron. (рис. -@fig:005)

![Каталог  var](https://github.com/Strikoder/OS/blob/main/lab%2005/report/img/5.5.JPG?raw=true) { #fig:005 width=70% }

2.3 Домашний каталог и его содержимое. (рис. -@fig:006)

![дом. кат.](https://github.com/Strikoder/OS/blob/main/lab%2005/report/img/5.6.JPG?raw=true) { #fig:006 width=70% }

1. Выполнил следующие действия:

3.1 Создал новый каталог с именем newdir 

3.2 Создал новый каталог с именем morefun в ~/newdir 

3.3 Создал одной командой три новых каталога с именами letters , memos , misk и удалил эти каталоги (рис. -@fig:007)


![каталог](https://github.com/Strikoder/OS/blob/main/lab%2005/report/img/5.7.JPG?raw=true) { #fig:007 width=70% }



5. Команда ls для просмотра содержимое не только указанного каталога, но и подкаталогов, входящих в него, с помощью man. (рис. -@fig:008)

![команда man](https://github.com/Strikoder/OS/blob/main/lab%2005/report/img/5.8%20manls.JPG?raw=true) { #fig:008 width=70% }



1. Команда man для  mkdir , rmdir , rm.


- mkdir (рис. -@fig:009)

![команда man](https://github.com/Strikoder/OS/blob/main/lab%2005/report/img/5.9.JPG?raw=true) { #fig:009 width=70% }


- rmdir (рис. -@fig:010)

![команда man](https://github.com/Strikoder/OS/blob/main/lab%2005/report/img/5.10.JPG?raw=true) { #fig:010 width=70% }


- rm (рис. -@fig:011)

![команда man](https://github.com/Strikoder/OS/blob/main/lab%2005/report/img/5.11.JPG?raw=true) { #fig:011 width=70% }


* Команда history (рис. -@fig:012)

![команда history](https://github.com/Strikoder/OS/blob/main/lab%2005/report/img/5.11%20history.JPG?raw=true) { #fig:012 width=70% }


# Контрольные вопросы

1. Командная строка является программной оболочкой позволяющей в текстовом виде вводить компьютеру различные команды.
2. Aбсолютный путь к текущему каталогу можно определить с помощью команды pwd.
3. При помощи команды ls и опции -F можно определить только тип файлов и их имена в текущем каталоге.
4. Некоторые файлы в операционной системе скрыты от просмотра и обычно используются для настройки рабочей среды. Имена таких файлов начинаются с точки. Для того, чтобы отобразить имена скрытых файлов, необходимо использовать команду ls с опцией -a.
5. Команда rm используется для удаления файлов и/или каталогов.
6. Команда history выводит список ранее выполненных команд.
7. Можно модифицировать команду из выведенного на экран списка при помощи следующей конструкции:
!<номер_команды>:s/<что_меняем>/<на_что_меняем>
Пример:
``!3:s/a/F ``
8. «;». Если требуется выполнить последовательно несколько команд, записанный в одной строке, то для этого используется символ точка с запятой
Пример:
``cd; ls``
9. Экранирование символов — замена в тексте управляющих символов на соответствующие текстовые подстановки. Если в встречаются специальные символы (типа «.», «/», «*» и т.д.), надо перед ними поставить символ экранирования \ (обратный слэш).
10. Чтобы вывести на экран подробную информацию о файлах и каталогах, необ-
ходимо использовать опцию l. При этом о каждом файле и каталоге будет выведена следующая информация:
– тип файла,
– право доступа,
– число ссылок,
– владелец,
– размер,
– дата последней ревизии,
– имя файла или каталога.
11. Относительный путь представляет собой путь по отношению к текущему рабочему каталогу пользователя или активных приложений. Используется в команде cd. 
12. Команда man используется для просмотра (оперативная помощь) в диалоговом режиме руководства (manual) по основным командам операционной системы типа Linux.
13. TAb служит для автоматического дополнения вводимых команд.

# Выводы

В ходе выполнения лабораторных работ я научился использовать некоторые команды ``ls``, ``mkdir``, ``cd``, ``man``. С небольшим или без каких-либо трудностей я смог выполнить лабораторные упражнения
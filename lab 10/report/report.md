---
# Front matter
lang: ru-RU
title: "Шаблон отчёта по лабораторной работе № 10"
subtitle: "Операционные Системы"
author: "Яссин мохамад аламин"
Group: "НКНбд-01-20"

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

# Цель работы

Познакомиться с операционной системой Linux. Получить практические навыки работы с редактором Emacs.


# Выполнение лабораторной работы

1. Открыл emacs.
(рис. -@fig:001)
![emacs](img/1.jpg) 
{ #fig:001 width=70% }

2. Создал файл lab07.sh с помощью комбинации ``Ctrl-x`` ``Ctrl-f`` (C-x C-f).

3. Набрал текст
(рис. -@fig:002)
![Введение текста](img/2.jpg) 
{ #fig:002 width=70% }

4. Сохранил файл с помощью комбинации Ctrl-x Ctrl-s (C-x C-s).

5. Проделать с текстом стандартные процедуры редактирования, каждое действие должно осуществляться комбинацией клавиш.

5.1. Вырезал одной командой целую строку (С-k).
(рис. -@fig:003)
![редактирование](img/3.jpg) 
{ #fig:003 width=70% }

5.2. Вставил эту строку в конец файла (C-y).
(рис. -@fig:004)
![редактирование](img/4.jpg) 
{ #fig:004 width=70% }

5.3. Выделил область текста (C-space).

5.4. Скопировал область в буфер обмена (M-w).

5.5. Вставил область в конец файла.

5.6. Вновь выделить эту область и на этот раз вырезать её (C-w).
(рис. -@fig:005)
![редактирование](img/5.jpg) 
{ #fig:005 width=70% }

5.7. Отменил последнее действие (C-/).


6. Научитесь использовать команды по перемещению курсора.

6.1. Переместил курсор в начало строки (C-a).

6.2. Переместил курсор в конец строки (C-e).

6.3. Переместил курсор в начало буфера (M-<).

6.4. Переместил курсор в конец буфера (M->).

7. Управление буферами.

7.1. Вывел список активных буферов на экран (C-x C-b).
(рис. -@fig:006)
![Управление буферами](img/6.jpg) 
{ #fig:006 width=70% }

7.2. Переместился во вновь открытое окно (C-x) o со списком открытых буферов и переключитесь на другой буфер.

7.3. Закрыл это окно (C-x 0).

7.4. Теперь вновь переключайтесь между буферами, но уже без вывода их списка на экран (C-x b).

1. Управление окнами.

8.1. Поделил фрейм на 4 части: разделите фрейм на два окна по вертикали(C-x 3), а затем каждое из этих окон на две части по горизонтали (C-x 2)



8.2. В каждом из четырёх созданных окон открыл новый буфер (файл) и ввел несколько строк текста.
(рис. -@fig:007)
![Управление окнами](img/10.jpg) 
{ #fig:007 width=70% }


1. Режим поиска
9.1. Переключился в режим поиска (C-s) и нашел несколько слов, присутствующих в тексте.
(рис. -@fig:008)
![Режим поиска](img/9.jpg) 
{ #fig:008 width=70% }

9.2. Переключился между результатами поиска, нажимая C-s.

9.3. Вышел из режима поиска, нажав C-g.

9.4. Перешел в режим поиска и замены (M-%), ввел текст, который следует найти и заменить, нажимал ``Enter`` , затем ввел текст для замены. После того как будут подсвечены результаты поиска, нажмите ``!`` для подтверждения замены.

9.5. Испробовал другой режим поиска, нажав M-s o. Объясните, чем он отличается от обычного режима?
``M-s`` сразу перешел к тому месту, где находится ввденное слово

# Контрольные вопросы

1. Emacs представляет собой мощный экранный редактор текста, написанный на языке высокого уровня Elisp.
2. 
3. Буфер — объект, представляющий какой-либо текст.
	Окно — прямоугольная область фрейма, отображающая один из буферов.
4. 
5. Emacs использует буферы с именами, начинающимися с пробела, для внутренних целей. Отчасти он обращается с буферами с такими именами особенным образом -- например, по умолчанию в них не записывается информация для отмены изменений
6. ``Ctrl`` + ``c``, а потом ``|`` и  ``Ctrl`` + ``c``  ``Ctrl`` + ``|``
7. Разделите фрейм на два окна по вертикали(``C-x`` 3), а затем каждое из этих окон на две части по горизонтали (``C-x`` 2).
8. Настройки emacs хранятся в файле . emacs, который хранится в домашней дирректории пользователя. Кроме этого файла есть ещё папка . emacs.
9. 
10. 
# Выводы

Познакомился с операционной системой Linux. Получил практические навыки работы с редактором Emacs.
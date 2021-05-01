---
# Front matter
lang: ru-RU
title: "Шаблон отчёта по 2 лабораторной работе"
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

# Отчёт о выполнении лабораторной работы №2 


# Цель работы

Изучить идеологию и применение средств контроля версий.
Научиться использовать систему контроля версии в своих проектах

# Задание

Настроить git на своем компьютере, инициализировать локальный репозиторий в папке с лабораторными работами,
добавить все нужные файлы в репозиторий, подключить удаленный репозиторий с github, связать локальный и удаленные репозитории


# Выполнение лабораторной работы
- На моем личном компьютере система Git и Gitflow уже их устанавил

- Создание ssh для подключения к репо без записи имени пользователя и пароля каждый раз
![ssh key](img/2.1.jpg)
- добавление безопасного ключа на github
![git-ssh key](img/2.2.jpg)
- создание нового репозитория
![New repo](img/2.3.jpg)
- добавление лицензии
![Licence](img/2.4.jpg)
- добавление файла git-ignore
![git-ignore](img/2.5.jpg)
- закинуть файл в гитхаб
![uploading files](img/2.6.jpg)
- используя git-flow
![using gitflow](img/2.7.jpg)
- добавление файлов и завершение релиза
![Release](img/2.8.jpg)
- отправка файлов в GitHub
![Github push](img/2.9.jpg)
- Файлы на github
![Files](img/2.10.jpg)


# Выводы
В этой лабораторной работе я научился использовать Git, 
и подключать удаленные репозитории, добавлять и удалять необходимые файлы.
Я также научился использовать Git Flow, который значительно упрощает разработку проекта и навигацию между ветвями.

# Контрольные вопросы

1. Системы контроля версий -VCS- это программное обеспечение, которое используется для облегчения работы с изменяющейся информацией, обычно - в проектах. Чаще всего используется при разработке, когда над одним проектом работает большое количество людей.
2.
- Репозиторий в системе контроля версий - Это удаленный репозиторий, в котором хранятся все файлы проекта
- commit - фиксирует изменения перед загрузкой файлов в систему контроля версий
- история хранит все изменения в проекте, и при необходимости позволяет откатиться в желаемое место
- рабочая копия - - это копия проекта на компьютере разработчика. Если другой член команды изменил проект, вам необходимо скачать новую версию проекта на свой компьютер.
3. В отличие от классических, в распределённых системах контроля версий центральный репозиторий не является обязательным. Среди классических VCS наиболее известны CVS, Subversion, а среди распределённых — Git, Bazaar, Mercurial. Принципы их работы схожи, отличаются они в основном синтаксисом используемых в работе команд.
В децентрализованных системах у каждого из участников проекта есть полная копия проекта на своем компьютере, что делает его менее зависимым от сервера (Git).
4. Для начала необходимо создать и подключить удаленный репозиторий. Затем, поскольку никто, кроме вас, не изменяет проект, по мере изменения проекта отправляйте изменения на сервер, и нет необходимости загружать изменения.
5. Участник проекта (пользователь) перед началом работы посредством определённых команд получает нужную ему версию файлов. После внесения изменений, пользователь размещает новую версию в хранилище. При этом предыдущие версии не удаляются из центрального хранилища и к ним можно вернуться в любой момент.
6. Упрощение обмена информацией, ускорение разработки, устранение ошибок и недочетов при разработке.
7.
- git init - инициализирует локальный репозиторий
- git add * или add. - добавляет файлы в репозиторий
- git commit - версия фиксации
- git pull - загружает текущую версию проекта
- git push - отправляет измененный проект на сервер
- git checkout - позволяет переключаться между ветками
- git status - текущий статус проекта
- git branch - просмотреть доступные ветки
- git remote add - добавить удаленный репозиторий
8. git push --all (push origin master/любой branch)
   
9.  Ветви функций, также иногда называемые ветвями тем, используются для разработки новых функций, которые должны появиться в текущих или будущих выпусках.
    
10. Существуют временные и системные файлы, которые загромождают проект и не нужны. путь к ним можно добавить в файл .gitignore, тогда они не будут добавлены в проект
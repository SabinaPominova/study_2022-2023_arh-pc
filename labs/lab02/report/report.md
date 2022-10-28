---
## Front matter
title: "Шаблон отчёта по лабораторной работе номер 2"
subtitle: "истема контроля версий Git"
author: "Поминова Сабина Александровна"

## Generic otions
lang: ru-RU
toc-title: "Содержание"

## Bibliography
bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl

## Pdf output format
toc: true # Table of contents
toc-depth: 2
lof: true # List of figures
lot: true # List of tables
fontsize: 12pt
linestretch: 1.5
papersize: a4
documentclass: scrreprt
## I18n polyglossia
polyglossia-lang:
  name: russian
  options:
	- spelling=modern
	- babelshorthands=true
polyglossia-otherlangs:
  name: english
## I18n babel
babel-lang: russian
babel-otherlangs: english
## Fonts
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase,Scale=0.9
## Biblatex
biblatex: true
biblio-style: "gost-numeric"
biblatexoptions:
  - parentracker=true
  - backend=biber
  - hyperref=auto
  - language=auto
  - autolang=other*
  - citestyle=gost-numeric
## Pandoc-crossref LaTeX customization
figureTitle: "Рис."
tableTitle: "Таблица"
listingTitle: "Листинг"
lofTitle: "Список иллюстраций"
lotTitle: "Список таблиц"
lolTitle: "Листинги"
## Misc options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Целью работы является изучить идеологию и применение средств контроля
версий. Приобрести практические навыки по работе с системой git

# Задание

Здесь приводится описание задания в соответствии с рекомендациями
методического пособия и выданным вариантом.

# Теоретическое введение

Здесь описываются теоретические аспекты, связанные с выполнением работы.

Например, в табл. [-@tbl:std-dir] приведено краткое описание стандартных каталогов Unix.

: Описание некоторых каталогов файловой системы GNU Linux {#tbl:std-dir}

| Имя каталога | Описание каталога                                                                                                          |
|--------------|----------------------------------------------------------------------------------------------------------------------------|
| `/`          | Корневая директория, содержащая всю файловую                                                                               |
| `/bin `      | Основные системные утилиты, необходимые как в однопользовательском режиме, так и при обычной работе всем пользователям     |
| `/etc`       | Общесистемные конфигурационные файлы и файлы конфигурации установленных программ                                           |
| `/home`      | Содержит домашние директории пользователей, которые, в свою очередь, содержат персональные настройки и данные пользователя |
| `/media`     | Точки монтирования для сменных носителей                                                                                   |
| `/root`      | Домашняя директория пользователя  `root`                                                                                   |
| `/tmp`       | Временные файлы                                                                                                            |
| `/usr`       | Вторичная иерархия для данных пользователя                                                                                 |

Более подробно об Unix см. в [@gnu-doc:bash;@newham:2005:bash;@zarrelli:2017:bash;@robbins:2013:bash;@tannenbaum:arch-pc:ru;@tannenbaum:modern-os:ru].

# Выполнение лабораторной работы

Задание 1.
Создаю учётную запись на сайте https://github.com/ и заполняю основные
данные. (рис. [-@fig:001])

![1.png](image/1.png){ #fig:001 width=90% }

Задание 2.
Делаю предварительную конфигурацию git. Настраиваю utf-8 в выводе сообщений git:
Задаю имя начальной ветки (будем называть её master), параметр autocrlf, параметр
safecrlf:

![11.png](image/11.png){ #fig:011 width=90% }
![12.png](image/12.png){ #fig:012 width=90% }

Задание 3.
Создаю SSH ключ

![13.png](image/13.png){ #fig:013 width=90% }

Задание 4.
Создаю рабочего пространства и репозитория курса на
основе шаблона.

![14.png](image/14.png){ #fig:014 width=90% }

Задание 5.
Создаю репозиторий курса на основе шаблона.
Репозиторий на основе шаблона можно создаю через web-интерфейс github.
Перехожу на станицу репозитория с шаблоном курса https://github.com/yam
adharma/course-directory-student-template.
Далее выбираю Use this template.

![15.png](image/15.png){ #fig:015 width=90% }

Далее создаю репозиторий

![3.png](image/3.png){ #fig:003 width=90% }

Задание 6.
Настраивю каталог курса

![4.png](image/4.png){ #fig:004 width=90% }

Отправляю все файлы на сервер 
![7.png](image/7.png){ #fig:007 width=90% }
# Выводы

Здесь кратко описываются итоги проделанной работы.

# Список литературы{.unnumbered}

::: {#refs}
:::

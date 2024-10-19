---
## Front matter
title: "Отчет по выполнению Индивидуального Проекта, Этап №3"
author: "Лобов Михаил Сергеевич"

## Generic options
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
mainfont: IBM Plex Serif
romanfont: IBM Plex Serif
sansfont: IBM Plex Sans
monofont: IBM Plex Mono
mathfont: STIX Two Math
mainfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
romanfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
sansfontoptions: Ligatures=Common,Ligatures=TeX,Scale=MatchLowercase,Scale=0.94
monofontoptions: Scale=MatchLowercase,Scale=0.94,FakeStretch=0.9
mathfontoptions:
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

Добавить содержимое на сайт

# Задание

1. Разместить краткое описание владельца сайта (Biography).
2. Добавить информацию об интересах (Interests).
3. Добавить информацию об образовании (Education).
4. Сделать пост по прошедшей неделе.
5. Добавить пост на тему по выбору:
   1. Легковесные языки разметки.
   2. Языки разметки. LaTeX.
   3. Язык разметки Markdown.

## Выполнение задач

### 1. Краткое описание владельца сайта (Biography)

Добавлено краткое биографическое описание владельца сайта. В нем представлены основные факты о карьере и личной жизни, а также профессиональные достижения. Особое внимание уделено проектам, над которыми велась работа, включая программирование и разработку веб-сайтов.

### 2. Информация об интересах (Interests)

В разделе "Интересы" были добавлены увлечения владельца сайта. Указаны как профессиональные направления, так и личные интересы, такие как программирование, веб-разработка, и изучение новых технологий. Также представлены хобби, такие как настольные игры и музыка, что добавляет индивидуальности и уникальности профилю владельца.

### 3. Информация об образовании (Education)

Добавлена информация об академическом образовании владельца сайта, включая учебные заведения, полученные дипломы и сертификаты. Отдельно отмечены достижения, такие как отличные оценки и участие в проектах на курсах по программированию и кибербезопасности.

### 4. Пост по прошедшей неделе

Были изменены файлы в директориях `C:\Users\kotof\HugoPrj\PepsiMonster.github.io\content\post\get-started` и `C:\Users\kotof\HugoPrj\PepsiMonster.github.io\content\post\project-management`, где я отредактировал .md файлы и добавил соответствующие изображения. 

Для поста "Project Management" был добавлен отчет, который включал описание выполненных задач:
- Генерация матрицы случайных чисел и их визуализация.
- Построение гистограммы нормального распределения случайных чисел.
- Моделирование случайной точки в пространстве.
- Алгоритмическая секция группового проекта была выполнена и оформлена в презентацию.
- Самостоятельно были изучены особенности языка SQL для бизнес аналитики.

Отчет кратко резюмировал выполненную работу и представил важные выводы по каждому этапу.

## Выводы

В рамках данной работы были добавлены ключевые элементы на сайт, что улучшило его функциональность и наполнило содержимым. Все задачи выполнены в соответствии с требованиями.

# Список литературы{.unnumbered}

::: {#[Индивидуальный проект №2](https://pepsimonster.github.io/)}
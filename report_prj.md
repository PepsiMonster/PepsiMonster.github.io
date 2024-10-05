---
## Front matter
title: "Отчет по выполнению Индивидуального Проекта, Этап №2"
author: "Лобов Михаил Сергеевич"

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

Добавить содержение на сайт

# Задание

1. Разместить фотографию владельца сайта.
2. Разместить краткое описание владельца сайта (Biography).
3. Добавить информацию об интересах (Interests).
4. Добавить информацию от образовании (Education).
5. Сделать пост по прошедшей неделе.
6. Добавить пост на тему по выбору:
   1. Управление версиями. Git.
   2. Непрерывная интеграция и непрерывное развертывание (CI/CD).

## Добавление материала

Git — это распределённая система управления версиями, которая позволяет разработчикам эффективно отслеживать изменения в коде и работать над проектами в команде. Основные преимущества Git заключаются в возможности сохранять историю изменений, работать с разными ветками и легко возвращаться к предыдущим состояниям проекта.

Ключевые команды Git:
git init — инициализация нового репозитория.

git clone — клонирование удалённого репозитория.

git add — добавление изменений в индекс (подготовка к коммиту).

git commit — создание коммита, который сохраняет изменения с сообщением.

git push — отправка изменений на удалённый сервер.

git pull — получение обновлений из удалённого репозитория и объединение их с локальными изменениями.

git status — проверка текущего состояния репозитория.

git log — просмотр истории изменений.

Git делает возможным параллельную работу над одним проектом, позволяет откатываться на предыдущие версии и разрешать конфликты при слиянии изменений. Это важный инструмент в арсенале каждого разработчика для организации и контроля разработки проекта.


# Выполнение лабораторной работы

В рамках выполнения лабораторной работы были реализованы следующие задачи:

Размещение фотографии владельца сайта: На главной странице была добавлена фотография владельца сайта в оптимизированном формате для быстрой загрузки и удобного отображения на различных устройствах.

Добавление краткого описания (Biography): Размещено краткое описание владельца сайта, содержащее основные факты и достижения, с акцентом на личные и профессиональные качества.

Информация об интересах (Interests): В отдельном разделе была добавлена информация об увлечениях владельца сайта, включая хобби, профессиональные интересы и направления для дальнейшего развития.

Информация об образовании (Education): В разделе "Образование" представлена информация о пройденных учебных заведениях, полученных дипломах и академических достижениях.

Пост о прошедшей неделе: Создан и опубликован пост, в котором освещаются ключевые события прошедшей недели, включая рабочие задачи, личные успехи и профессиональные достижения.

Все задачи лабораторной работы были выполнены в соответствии с требованиями, результат представлен на сайте в виде организованных и легко доступных разделов.


# Выводы

По итогу проделанной работы были сайт на hugo дополнен разным контентом. 

# Список литературы{.unnumbered}

::: {#[Индивидуальный проект №2](https://pepsimonster.github.io/)}
:::
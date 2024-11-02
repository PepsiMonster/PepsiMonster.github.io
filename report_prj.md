---
## Front matter
title: "Отчет по Индивидуальному проекту №4 по предмету Научное программирование"
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

# Отчет по индивидуальному проекту этап 4

## Цель работы

Цель данной работы — создать и разместить на сайте новые посты, включая **посты о событиях прошедшей недели** и об **оформлении отчетов**, а также добавить ссылки на различные исследовательские ресурсы. Эти задачи помогают структурировать и улучшить содержание сайта, а также добавить важные ссылки для академической и исследовательской работы.

## Задание

1. Зарегистрироваться на соответствующих ресурсах и разместить на них ссылки на сайте:
   - eLibrary : [https://elibrary.ru/](https://elibrary.ru/)
   - Google Scholar : [https://scholar.google.com/](https://scholar.google.com/)
   - ORCID : [https://orcid.org/](https://orcid.org/)
   - Mendeley : [https://www.mendeley.com/](https://www.mendeley.com/)
   - ResearchGate : [https://www.researchgate.net/](https://www.researchgate.net/)
   - Academia.edu : [https://www.academia.edu/](https://www.academia.edu/)
   - arXiv : [https://arxiv.org/](https://arxiv.org/)
   - GitHub : [https://github.com/](https://github.com/)
2. Создать пост по событиям прошедшей недели.
3. Добавить пост на тему по выбору: оформление отчетов.

## Теоретическое введение

Для создания сайта использовался генератор сайтов **Hugo** с темой **Academic CV**, который поддерживает настройку постов и добавление изображений через Front matter. Система Hugo позволяет создавать и организовывать контент, используя Markdown, а также легко добавлять ссылки и изображения, что делает её удобной для ведения личного блога или сайта.

### Front matter и структура постов

Front matter — это начальный блок параметров в каждом Markdown-файле Hugo. Он позволяет задать заголовок, автора, теги, изображения и другие настройки поста. Например, параметр `image: featured` задаёт изображение, которое будет отображаться на странице поста, добавляя визуальную привлекательность контенту.

### Регистрация на ресурсах и добавление ссылок

Ссылки на научные ресурсы помогают пользователям сайта быстро находить важные академические и исследовательские платформы. Эти ссылки были добавлены на сайт, чтобы облегчить доступ к источникам для тех, кто хочет публиковаться, искать научные статьи и следить за последними исследованиями.

## Выполнение лабораторной работы

#### 1. Регистрация и добавление ссылок на ресурсы

Я зарегистрировался на платформах **eLibrary**, **Google Scholar**, **ORCID**, **Mendeley**, **ResearchGate**, **Academia.edu**, **arXiv** и **GitHub**. После этого я добавил ссылки на данные ресурсы на сайте, создав раздел для быстрого доступа к этим платформам. Это добавило удобства для пользователей сайта, поскольку они могут быстро переходить на исследовательские ресурсы.

#### 2. Создание поста о событиях прошедшей недели

Для поста о событиях прошедшей недели я создал новую папку `Week4Post` в директории `content/posts/`, внутри которой разместил Markdown-файл `index.md` и изображение `featured.jpg` для украшения поста.

Пример Front matter для поста:

```markdown
---
title: "✅ Пост по событиям прошедшей недели"
summary: "Вам же не терпится узнать, что произошло у меня на этой неделе? 😘"
date: 2024-11-02
authors:
  - admin
tags:
  - Weekly post
  - Markdown
image:
  featured: '/post/Week4Post/featured.jpg'
---
```

Этот файл содержит краткое описание (`summary`), теги (`tags`) и путь к изображению (`image: featured`). После добавления этого файла и изображения я запустил сайт с помощью Hugo, чтобы убедиться, что пост и изображение отображаются корректно.

#### 3. Создание поста на тему "Оформление отчёта"

Кроме того, я создал пост на тему "Оформление отчета", где подробно описал структуру отчета, использование Front matter, разделы и элементы Markdown. Для этого я создал новую папку в `content/posts/`, разместив там файл `ReportWriting.md` с описанием оформления отчетов. Этот пост ориентирован на студентов и исследователей, которые хотят узнать, как создавать структурированные и профессионально оформленные отчеты в Markdown.

Пример Front matter для поста о написании отчетов:

```markdown
---
title: "Как написать отчет в Markdown: Полное руководство"
summary: "Полезные советы по оформлению отчетов с использованием Markdown и Hugo"
date: 2024-11-02
authors:
  - admin
tags:
  - Second Brain
  - Markdown
image:
  featured: '/post/ReportWriting/featured.jpg'
---
```

# Выводы

В ходе выполнения данной работы были созданы два новых поста, один из которых посвящен событиям прошедшей недели, а другой — теме оформления отчетов. Также были добавлены ссылки на популярные исследовательские платформы, что сделало сайт более полезным и функциональным для его посетителей. Эти задачи помогли мне лучше понять структуру и работу с контентом в Hugo, а также улучшить навыки оформления и создания постов в Markdown.

# Список литературы

1. Официальная документация Hugo: [https://gohugo.io/documentation/](https://gohugo.io/documentation/)
2. Markdown Guide: [https://www.markdownguide.org/](https://www.markdownguide.org/)
3. Официальные сайты академических платформ (eLibrary, Google Scholar, ORCID и другие).



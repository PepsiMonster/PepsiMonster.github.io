---
title: ✅ Написание отчетов
summary: Руководство по написанию отчетов в markdown!
date: 2024-11-02
authors:
  - admin
tags:
  - Hugo Blox
  - Markdown
image:
  #caption: 'Image credit: [**Unsplash**](https://unsplash.com)'
  featured: '/images/featured.jpg'
---

```markdown
# Как написать отчет в Markdown: Полное руководство

Написание отчетов в формате Markdown — это простой и удобный способ структурировать и оформить документацию. В этом посте я покажу, как правильно оформить отчет, используя **Front matter** и основные разделы отчета. Пример отчета ниже демонстрирует структуру и форматирование, которые помогут вам создать профессионально оформленный документ.

## Front matter: основа оформления отчета

Front matter — это специальный блок настроек в начале Markdown-документа, который помогает задать параметры для форматирования и оформления. Он включает в себя метаданные и технические параметры для создания PDF-файла или другого выходного формата.

### Пример Front matter

Пример стандартного **Front matter** для отчета выглядит так:

```markdown
---
title: "Отчет по Лабораторной работе №2 по предмету Математические основы защиты информации и информационной безопасности"
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
```

### Пояснения к Front matter

- **title**: Название отчета, которое будет отображаться на титульной странице.
- **author**: Имя автора отчета.
- **lang**: Установка языка документа (в данном случае — русский).
- **toc-title**: Название для содержания.
- **bibliography** и **csl**: Пути к файлам для создания списка литературы в нужном стиле.
- **toc, toc-depth, lof, lot**: Настройки отображения содержания, списка иллюстраций и таблиц.
- **fontsize, linestretch, papersize**: Настройки шрифта, межстрочного интервала и размера страницы.
- **documentclass**: Класс документа для LaTeX (например, `scrreprt`).
- **polyglossia-lang, babel-lang**: Настройки языковых пакетов для многоязычного оформления.
- **Fonts**: Настройки основных, дополнительных и моноширинных шрифтов.
- **Biblatex**: Опции для библиографического стиля.
- **Misc options**: Дополнительные настройки, включая использование пакетов LaTeX для оформления.

Front matter задает основные параметры, обеспечивая красивое и структурированное оформление, особенно при экспорте в PDF.

---

## План отчета: структура и разделы

После настройки **Front matter** следует основной текст отчета, который обычно состоит из нескольких стандартных разделов.

### 1. Цель работы

Раздел **Цель работы** объясняет, зачем выполнялась лабораторная работа. Он может содержать одну-две фразы, описывающие основные задачи и цели.

**Пример:**
```markdown
# Цель работы

Цель данной работы — изучить шифры перестановки и реализовать их программное исполнение на языке Julia.
```

### 2. Задание

Раздел **Задание** описывает, что конкретно требуется выполнить в рамках лабораторной работы. Этот раздел может включать перечень задач, которые нужно решить.

**Пример:**
```markdown
# Задание

Программно реализовать на языке Julia шифры:
1. Маршрутное шифрование
2. Шифрование с помощью решеток
3. Таблица Виженера
```

### 3. Теоретическое введение

**Теоретическое введение** — это краткий обзор теории, связанной с темой лабораторной работы. Здесь приводятся основные понятия, формулы и алгоритмы, которые будут использованы в ходе работы.

**Пример:**
```markdown
# Теоретическое введение

## Маршрутное шифрование

Маршрутное шифрование представляет собой метод шифрования, при котором...
```

### 4. Выполнение лабораторной работы

В разделе **Выполнение лабораторной работы** подробно описываются все шаги, выполненные для решения задачи, а также приводится программный код и результаты выполнения. Также можно добавить скриншоты для наглядности.

**Пример:**
```markdown
# Выполнение лабораторной работы

Написаны программы на языке Julia.

![Маршрутное шифрование](pictures/Viettpic1.png){#fig:001 width=70%}
```

### 5. Выводы

В разделе **Выводы** описываются результаты, достигнутые в ходе выполнения лабораторной работы, а также дается краткая оценка эффективности использованных методов и средств.

**Пример:**
```markdown
# Выводы

По итогу проделанной работы были написаны 3 программы для каждого алгоритма шифрования...
```

### 6. Список литературы

**Список литературы** включает все источники, использованные при подготовке отчета. Этот раздел формируется автоматически, если в **Front matter** указаны параметры библиографического стиля.

**Пример:**
```markdown
# Список литературы{.unnumbered}

::: {#[Лабораторная_работа_2](https://esystem.rudn.ru/mod/folder/view.php?id=1150970)}
:::
```

---

## Заключение

Создание отчетов в Markdown с использованием **Front matter** и стандартной структуры позволяет легко оформлять документ для различных выходных форматов. Используя это руководство, вы сможете написать отчет, который будет соответствовать академическим стандартам и иметь профессиональный вид при экспорте в PDF или другой формат.
```
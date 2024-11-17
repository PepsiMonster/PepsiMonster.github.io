---
title: 👩🏼‍🏫 Преподавайте академические курсы
summary: Встраивайте видео, подкасты, код, математические формулы LaTeX и даже тестируйте студентов!
date: 2023-10-24
math: true
authors:
  - admin
tags:
  - Hugo
  - Hugo Blox Builder
  - Markdown
image:
  caption: 'Встраивайте мультимедиа, такие как видео и формулы LaTeX'
---

[Hugo Blox Builder](https://hugoblox.com) разработан для того, чтобы дать создателям технического контента удобный инструмент. Вы сосредотачиваетесь на содержимом, а Hugo Blox Builder, на основе которого создан этот шаблон, берёт на себя всё остальное.

**Встраивайте видео, подкасты, код, математические формулы LaTeX и даже тестируйте студентов!**

На этой странице представлены примеры технического контента, который можно отобразить с помощью Hugo Blox.

## Видео

Преподавайте свой курс, делясь видео со студентами. Выберите один из следующих подходов:

**YouTube**:

    {{</* youtube D2vj0WcvH5c */>}}

{{< youtube D2vj0WcvH5c >}}

**Bilibili**:

    {{</* bilibili BV1WV4y1r7DF */>}}

{{< bilibili BV1WV4y1r7DF >}}

**Видео-файл**

Видео можно добавить на страницу, разместив их в вашей библиотеке `assets/media/` или в [папке страницы](https://gohugo.io/content-management/page-bundles/), а затем встроив их с помощью шорткода _video_:

    {{</* video src="my_video.mp4" controls="yes" */>}}

## Подкасты

Вы можете добавить подкаст или музыкальный файл на страницу, разместив MP3-файл в папке страницы или в папке медиа-библиотеки, а затем встроив аудио с помощью шорткода _audio_:

    {{</* audio src="ambient-piano.mp3" */>}}

Попробуйте:

{{< audio src="ambient-piano.mp3" >}}

## Тестирование студентов

Предоставьте простую, но интересную самооценку, открывая решения задач с помощью шорткода `spoiler`:

```markdown
{{</* spoiler text="👉 Нажмите, чтобы увидеть решение" */>}}
Вы нашли меня!
{{</* /spoiler */>}}
```

Отображается как:

{{< spoiler text="👉 Нажмите, чтобы увидеть решение" >}} Вы нашли меня 🎉 {{< /spoiler >}}

## Математика

Hugo Blox Builder поддерживает расширение Markdown для математических формул $\LaTeX$. Включите поддержку математики, добавив параметр `math: true` в заголовок страницы или включив её для всего сайта в файле `config/_default/params.yaml`:

```yaml
features:
  math:
    enable: true
```

Для отображения _встроенной_ или _блочной_ математики заключите формулы LaTeX в `$...$` или `$$...$$` соответственно.

Пример **блочной математики**:

```latex
$$
\gamma_{n} = \frac{ \left | \left (\mathbf x_{n} - \mathbf x_{n-1} \right )^T \left [\nabla F (\mathbf x_{n}) - \nabla F (\mathbf x_{n-1}) \right ] \right |}{\left \|\nabla F(\mathbf{x}_{n}) - \nabla F(\mathbf{x}_{n-1}) \right \|^2}
$$
```

Отображается как:

$$\gamma_{n} = \frac{ \left | \left (\mathbf x_{n} - \mathbf x_{n-1} \right )^T \left [\nabla F (\mathbf x_{n}) - \nabla F (\mathbf x_{n-1}) \right ] \right |}{\left \|\nabla F(\mathbf{x}_{n}) - \nabla F(\mathbf{x}_{n-1}) \right \|^2}$$

Пример **встроенной математики** `$\nabla F(\mathbf{x}_{n})$` отображается как $\nabla F(\mathbf{x}_{n})$.

Пример **многострочной математики** с использованием разрыва строк (`\\`):

```latex
$$f(k;p_{0}^{*}) = \begin{cases}p_{0}^{*} & \text{if }k=1, \\
1-p_{0}^{*} & \text{if }k=0.\end{cases}$$
```

Отображается как:

$$
f(k;p_{0}^{*}) = \begin{cases}p_{0}^{*} & \text{if }k=1, \\
1-p_{0}^{*} & \text{if }k=0.\end{cases}
$$

## Код

Hugo Blox Builder использует расширение Markdown от Hugo для подсветки синтаксиса кода. Тему подсветки можно выбрать в файле `config/_default/params.yaml`.

    ```python
    import pandas as pd
    data = pd.read_csv("data.csv")
    data.head()
    ```

Отображается как:

```python
import pandas as pd
data = pd.read_csv("data.csv")
data.head()
```

## Встроенные изображения

```go
{{</* icon name="python" */>}} Python
```

Отображается как:

{{< icon name="python" >}} Python

## Эта страница оказалась полезной? Поделитесь ею 🙌

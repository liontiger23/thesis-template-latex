---
documentclass: extarticle
papersize: a4
geometry: "left=3cm,right=2cm,top=3cm,bottom=2cm"

fontsize: 14pt
listings: true
indent: true
codeBlockCaptions: true
colorlinks: false
link-citations: true

mainfont: Times New Roman
monofont: DejaVu Sans Mono
mathfont: XITS Math
lang: ru-RU
babel-lang: russian

figPrefix: 
  - рис.
  - рис.
tblPrefix: 
  - табл.
  - табл.
toc-title: СОДЕРЖАНИЕ

# Comment out if title is not needed
include-before: |
  ```{=latex}
  \includepdf[pages={1}]{src/title.pdf}
  ```
---

\pagebreak
# ВВЕДЕНИЕ {#sec:introduction -}

Данная работа является примером оформления текста ВКР.
В качестве примера ссылки на литературу, можно упомянуть язык Java [@gosling2000java],
который исполняется на виртуальной машине JVM [@lindholm2014java].

Завершение введения отдельным параграфом.

\clearpage
\pagebreak
# ПОСТАНОВКА ЗАДАЧИ {#sec:overview}

Постановка задачи и обзор существующих работ.

## Теорема Пифагора

Основная формулировка содержит алгебраические действия ---
в прямоугольном треугольнике, длины катетов которого равны 
$a$ и $b$, а длина гипотенузы --- $c$, выполнено соотношение:

$$
a^2 + b^2 = c^2.
$$

Для того чтобы ссылаться на формулы, их можно нумеровать следующим образом:

$$
a^2 + b^2 = c^2
$$ {#eq:pythagoras}

На такую формулу можно ссылаться как [-@eq:pythagoras] где угодно в тексте.

## Пример листинга

Ниже в листинге [-@lst:python-fact] представлен пример
вычисления факториала на языке Python.

```{.python #lst:python-fact}
def fact(n):
  if (n==1 or n==0):
    return 1
  else:
    return n * fact(n - 1)
```
: Вычисление факториала числа `n`

## Пример рисунка

Далее на рис. [-@fig:png-svg-compare] и [-@fig:tikz-example] представлены
примеры вставки изображений в работу.

<div id="fig:png-svg-compare">

![](images/sample/Markdown-mark.svg.png){#fig:markdown-mark-png width=40%}
![](images/sample/Markdown-mark.pdf){#fig:markdown-mark-svg}

Пример рисунка в формате png [-@fig:markdown-mark-png]
и в формате svg после конвертации в pdf [-@fig:markdown-mark-svg]
</div>

```{=latex}
\begin{tikzfigure}{fig:tikz-example}{Таблица виртуальных методов для класса C}
  {every node/.style={text=black}}

  \begin{scope}[blend group = soft light]
    \fill[red!30!white]   ( 90:1.2) circle (2);
    \fill[green!30!white] (210:1.2) circle (2);
    \fill[blue!30!white]  (330:1.2) circle (2);
  \end{scope}
  \node at ( 90:2)    {Typography};
  \node at ( 210:2)   {Design};
  \node at ( 330:2)   {Coding};
  \node [font=\Large] {\LaTeX};

\end{tikzfigure}
```

\clearpage
\pagebreak
# РАЗРАБОТАННЫЙ ПОДХОД {#sec:solution}

\clearpage
\pagebreak
# ЗАКЛЮЧЕНИЕ {#sec:conclusion -}

Основные результаты работы:

- Первый результат;
- Второй результат;
- Третий результат;
- Последний результат.

Направление дальнейших работ:

- Улучшить алгоритм;
- Провести анализ данных.

\clearpage
\pagebreak
# СПИСОК ИСПОЛЬЗОВАННЫХ ИСТОЧНИКОВ {-}

<div id="refs"></div>

\renewcommand{\thesection}{П}
\setcounter{subsection}{0}
\setcounter{figure}{0}
\setcounter{lstlisting}{0}
\pagebreak
# ПРИЛОЖЕНИЕ {#sec:appendix -}

## Первая глава приложения

В приложение обычно выносятся длинные листинги и таблицы.






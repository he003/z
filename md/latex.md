% Latex CSS

::: {.abstract}
Robbin He

Nov 12, 2022

## Abstract
This almost class-less css libray turns your HTML document into a website which looks like a [Latex]{.latex} document.

Source code can be found [github](https://github.com/vincentdoerig/latex-css)
:::

## Dark mode

<button id="dark-mode-toggle">Toggle dark mode</button>

<script>
document
  .querySelector("#dark-mode-toggle")
  .addEventListener('click', () => {
     document.body.classList.toggle("latex-dark");
  });
</script>

## Getting started

- add css link to your doc
- (optional) add any classes to elements described in the **next section**
- (optional) add dark mode by add `latex-dark-auto` to `body` tag
- support math (pandoc support)
- syntax highlight (pandoc support)

## Theorems, Definitions, Lemmas and Proffs

::::::{#wrapper lang=zh-hans}

:::{.theorem}
The real numbers $\mathbb{R}$ are uncountable.
:::

:::{.proof}
If $\mathbb{R}$ is countable, then [0, 1] is countable a well. Hence there exists a map C from $\mathbb{N}$ onto [0, 1] with $$C(n) = \sum_{i=1}^{\infty} c_{i}(n) 10^{-i}$$ where $c_{i}(n)\in\{0,1, \ldots, 9\}$ are the digits in decimeal expansion.
:::

:::{.theorem}
If $S$ is both countable and infinite, then there is a bijection beteween $S$ and $\boldsymbol{N}$ itself.
:::

:::{.proof}
For any $s \in S,$, we let $f(s)$ denote the value of $k$ ...
:::

:::{.lemma}
An even number plus one even number results in a even number.
:::

:::{.definition}
A definition is a statement of the meaning of a word or word group or a sign or symbol.
:::

::::::

## SideNote

Here is a sidenote
<label for="sn-1" class="sidenote-toggle sidenote-number"></label>
<input type="checkbox" id="sn-1" class="sidenote-toggle" />
<span class="sidenote">side note content in right side</span>

Here is a another sidenote
<label for="sn-2" class="sidenote-toggle sidenote-number"></label>
<input type="checkbox" id="sn-2" class="sidenote-toggle" />
<span class="sidenote left">Here is the content for sidenote in left side.</span>

## Others

For long formula and table, please wrap them in div and add class `scroll-wrapper`.

Color Name      |Hex code
----------------|--------------------------------------------
[teal]{sytle='color: teal;'} | `#008080`
[goldenrod]{style='color: goldenrod;'} | `#daa520`
[cornflowerblue]{style='color: cornflowerblue;'} | `#6495ed`
[lightcoral]{style='color: lightcoral;'} | `#f08080`

Table: Color and values

# FAQ - EdStem Forum

- [FAQ - EdStem Forum](#faq---edstem-forum)
  - [Why do we use EdStem for the course and not Canvas discussion forum?](#why-do-we-use-edstem-for-the-course-and-not-canvas-discussion-forum)
  - [What are the expected behavior and etiquette rules for the forum?](#what-are-the-expected-behavior-and-etiquette-rules-for-the-forum)
  - [Is there a short guide/description for EdStem?](#is-there-a-short-guidedescription-for-edstem)
  - [EdStem can do Latex! How?](#edstem-can-do-latex-how)


## Why do we use EdStem for the course and not Canvas discussion forum?

It is nicer, faster, and more productive for everyone (students and staff).

Forums like EdStem and Piazza have not only increases engagement a lot (between 7x to 10x), but also are much much more productive for the teaching staff, which in turn allows staff to answer way many more questions and quicker, thus providing better service for more students.

We can start naming all the mamy things that EdStem does much better (nicer and more efficiently), but I leave it to you to find out... 😉

## What are the expected behavior and etiquette rules for the forum?

Please see dedicated [Forum FAQ & Etiquette](https://docs.google.com/document/d/1HdrY91LIPRZOEni_jsCwmN8Oc8MrUzljen6qHzbtQeU/edit?usp=sharing).


## Is there a short guide/description for EdStem?

Yes, refer to the [Quick Start Guide](https://edstem.org/quickstart/ed-discussion.pdf).


## EdStem can do Latex! How?

For those of you who are interested, you can use the typesetting language $\LaTeX$ very easily in your posts in Piazza by putting whatever you want to be converted between two sets of double dollar signs.

To give an example, typing:

```
$L_1 = {a^{2n}w \mid n \geq 0, w \in {b,c} \cup {\lambda}} = L((aa)^*(b \mid c \mid \lambda))$
```

will produce:

$L_1 = {a^{2n}w \mid n \geq 0, w \in {b,c}\cup {\lambda}} = L((aa)^*(b \mid c \mid \lambda))$

The symbol `$` opens a math environment: anything between `$` is treated as mathematic expressions.

You can even do more complicated things like this:

```
$$
\begin{array}{|c|c|}\hline
    \text{Symbol} & \text{Description}\\ \hline
    \mathbb{N} & \text{Natural numbers}\\
    \mathbb{Z} & \text{Integers}\\
    \mathbb{Q} & \text{Rational numbers}\\
    \mathbb{R} & \text{Real numbers}\\ \hline
\end{array}
$$
```

to produce this table:

$$
\begin{array}{|c|c|}\hline
\text{Symbol} & \text{Description}\\ \hline
\mathbb{N} & \text{Natural numbers}\\ 
\mathbb{Z} & \text{Integers}\\
\mathbb{Q} & \text{Rational numbers}\\ 
\mathbb{R} & \text{Real numbers}\\ \hline
\end{array}
$$

If you DO need to write `$` for whatever reason, you can "escape" the trigger for this by putting a backslash before each dollar sign, like `\$`.

If your plan is to go into research after this degree, then learning how to use Latex is almost essential, almost all Computer Science academic papers are written in Latex. But even if you aren't planning on going into research, it's pretty easy to pick up and it makes your uni assignments look very neat and professional, without having to put very much effort in at all (it would be especially useful to those of you who have Computing Theory in their program structure ;-) )

Anyway, it is not essential, so don't worry about it if you are already swamped under so much work that the prospect of learning something new and unnecessary is terrifying right now; but if you're like me and find these things interesting, you can get more information about the different commands and things you can do in the maths environment (with plenty of examples) here and here.

To get you started, some commands that you might find useful for this course are:

$\lambda$ - `\lambda`

$\epsilon$ - `\epsilon` (you can actually just type `\` and then any greek letter)

$\Sigma$ - `\Sigma` (if you capitalise the word, it gives you the capital greek letter)

$\rightarrow$ - `\rightarrow`

$\Rightarrow$ - `\Rightarrow` (capitalising arrows makes them double)

$\land$ - `\land`

$\lor$ - `\lor`

$\forall$ - `\forall`

$\exists$ - `\exists`

$\neg$ - `\neg`

$\cup$ - `\cup`

$\cap$ - `\cap`

$\subseteq$ - `\subseteq`

$\subset$ - `\subset`

$\neq$ - `\neq`

$\not=$ - `\not=` (you can use not with any other symbol and will cross it)

$\geq$ - `\geq`

$\leq$ - `\leq`

$\emptyset$ - `\emptyset`

$\infty$ - `\infty`

$\times$ - `\times`

$\mid$ - `\mid` (this is different to `|` as `(a|b)` will produce $(a|b)$ and `(a \mid b)` will produce $(a \mid b)$)

$a \cdot b$ - `a \cdot b`

$\dots$ - `\dots`

$\underline{a}$ - `\underline{a}`

$\overline{a}$ - `\overline{a}`

$a \in \{a,b,c\}$ - `a \in \{a,b,c\}`

$\not\in$ - `\not\in` (you can actually use `\not` for a lot of stuff such as `\not\subset` for $\not\subset$)

$a^x$ - `a^x` (you can use `^` to make a superscript of anything)

$a^{2n}$ - `a^{2n}` (if you need a superscript of more than one character, you need to use brackets otherwise you get $a^2n$)

$a_{bc}$ - `a_{bc}` (subscript is the same, brackets for more than one character)

${a}$ - `\{a\}` (to do set brackets, you need to escape them by using backslashes, otherwise it thinks the brackets are functional, as above)

$\mathbb{N}$ - `\mathbb{N}` (any letter can be substituted here)

$\frac{a}{b}$ - `\frac{a}{b}` (fractions you can put inline)

$\displaystyle\frac{a}{b}$ - `\displaystyle\frac{a}{b}` (`\displaystyle` gives you more space, but is usually used when you have equations on their own)

$\displaystyle\sum^{n+1}{i=0}2i$ - `\displaystyle\sum^{n+1}{i=0}2i` (without `\displaystyle` the sum would fit inline, the `^` is above and `_` for below)

$\text{this is text}$ - `\text{this is text}` (you need to use `\text{}` to write text inside a mathematical environment otherwise 'this is text' will say $this is text$)

That's about all i can think of off the top of my head that you will need.. if anyone has any more, feel free to reply here and we can build up a library.


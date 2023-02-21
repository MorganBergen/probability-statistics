## ch 03 random variables and probability distributions

**contents**

1.  [concept of a random variable](#concept-of-a-random-variable)
    - [definition 3.1](#definition-31)
    - [example 3.1](#example-31)
    - [example 3.3](#example-33)
    - [example 3.5](#example-35)
    - [discrete random variable](#discrete-random-variable)
    - [continuous random variable](#continuous-random-variable)
    - [definition 3.2 discrete sample space](#definition-32-discrete-sample-space)
    - [definition 3.3 continuous sample space](#definition-33-continuous-sample-space)
2.  [discrete probability distributions](#discrete-probability-distributions)
    - [definition 3.4 probability mass function](#definition-34-probability-mass-function)
    - [example 3.6](#example-36)
    - [example 3.8](#example-38)
    - [example 3.9](#example-39)
    - [definition 3.5](#definition-35)
    - [example 3.10](#example-310)
    - [figure probability mass function plot](#probability-mass-function-plot)
    - [figure probability histogram](#probability-histogram)
    - [figure discrete cumulative distribution function](#discrete-cumulative-distribution-function)
3.  [continuous probability distributions](#continuous-probability-distributions)
4.  [joint probability distributions](#joint-probability-distributions)
5.  [exercises](#exercises)

## concept of a random variable

- it is often important to allocate a numerical description to the outcome of a statistical experiment
- for a given sample space $S$ of some experiment, a random variable (rv) is any rule that associates a number with each outcome in $S$

### definition 3.1

**a random variable rv is a function that associates a real number with each element in the sample space**

- the function's domain is the sample space and it's range is the set of real numbers $\mathbb{R}$
- one and only one numerical value is assigned to each sample point x
- random variables are customarily denoted by upper case letters $X, Y, Z, \dots$
- we use lowercase letters to represent some particular value of the corresponding random variable
- the notation $X(\omega) = x$ means that $x$ is the value associated with the outcome $s$ by the rv $X$

### example 3.1

**two balls are drawn in succession without replacement from a box containing 4 red balls and 3 black balls.**

- the possible outcomes and the values y of the random variable Y, where Y is the number of red balls are

| sample space | y |
|:------------:|:-:|
|  RR          | 2 |
|  RB          | 1 |
|  BR          | 1 |
|  BB          | 0 |

**number of defective (D) products when 3 products are tested**

|sample space| x: values of X |
|:----------:|:--------------:|
| DDD        | 3              |
| DDN        | 2              |
| DND        | 2              |
| DNN        | 1              |
| NDD        | 2              |
| NDN        | 1              |
| NND        | 1              |
| NNN        | 0              |

### example 3.3 

**components from the production line are defective or not defective**

- define the random variable $X$ by

$$
f(x) = 
\begin{cases} 
        1, \text{ if the component is defective} \\
        0, \text{ if the component is not defective} \\
\end{cases}
$$

- this random variable is categorical in nature

### example 3.5
**a process will be evaluated by sampling items until a defective item is observed**

- define $X$ by the number of consecutive items observed

| sample space | x |
|:------------:|:-:|
| D            | 1 |
| ND           | 2 |
| NND          | 3 |
| ...          |  ... |


### discrete random variable

- according to the _countability_ of the sample space, which is measurable, it can be either discrete or continuous

- **discrete random variable** is a random variable whose sample space is discrete, if a random variable takes on only a countable number of distinct values
    - if the set of possible outcomes is countable
    - often this represents count data, such as the number of defectives, highway fatalities, etc.
-  a discrete random varibale assumes each of its values with a certain probability
-  frequently, it is convenient to represent all the probabilities of a random variable $X$ by a formula

$$f(x) = P(X = x), f(3) = P(X = 3)$$

### continuous random variable

- **continuous random variable** if a random variable can take on values on a continuous scale
    - often represents measured data, such as heights, weights, temperatures, distance, or life periods

### definition 3.2 discrete sample space

**discrete sample space**  if a sample space contains a _finite number of possibilities_ or an unending sequence with as many elements as there are whole numbers.

### definition 3.3 continuous sample space

**continuous sample space** if a sample space contains an _infinite_ number of possibilities equal to the number of points on a line segment.

### definition 3.4 probability mass function

**probability mass function** is the set of ordered pars $(x, f(x))$ is a probability function, probability mass function, or probability distribution of the discrete random variable $X$ if for each possible outcome $x$.

1.  $f(x) \geq 0$

2.  $\sum f(x) = 1$

3.  $P(X = x) = f(x)$

the probability distribution of a discrete random variable can be presented in the form of a mathematical formula, a table, or a graph-probability histogram, or barchart.

### example 3.6

let $X$ be the random variable:  number of heads in 3 tosses of a fair coin.

| sample space | x |
|:------------:|:-:|
| TTT          | 0 |
| TTH          | 1 |
| THT          | 1 |
| THH          | 2 |
| HTT          | 1 |
| HTH          | 2 |
| HHT          | 2 |
| HHH          | 3 |

the probability $P(X = x)$ that the outcome is a specific $x$ value is the probability that the number of heads is $x$.

| x | 0 | 1 | 2 | 3 |
|:-:|:-:|:-:|:-:|:-:|
| **$P(X = x)$** | 1/8 | 3/8 | 3/8 | 1/8 |

### example 3.8

-  a shipment of 8 similar microcomputers to a retail outlet contains 3 that are defective.  
-  if a school makes a random purchase of 2 of these computers
-  find the probability distribution for the number of defectives in the shipment

$$
f(0) = P(X = 0) = \frac{\binom{3}{0}\binom{5}{2}}{\binom{8}{2}} = \frac{10}{28} = 0.357 \\
$$
$$
f(1) = P(X = 1) = \frac{\binom{3}{1}\binom{5}{1}}{\binom{8}{2}} = \frac{15}{28} = 0.536 \\
$$
$$
f(2) = P(X = 2) = \frac{\binom{3}{2}\binom{5}{0}}{\binom{8}{2}} = \frac{3}{28} = 0.107 \\
$$

| x | 0 | 1 | 2 |
|:-:|:-:|:-:|:-:|
|**$f(x)$** | 10/28 | 15/28 | 3/28 |

### example 3.9

if a car agency sells 50% of its inventory of a certain foreign car equipped with side airbags, find the probability distribution of the number of cars with side airbags, find the probability distribution of the number of cars with side airbags, find the probability distribution of the number of cars with side airbags among the next 4 cars sold by the agency.

**solution** since the probability of selling an automobile with side airbags is 0.5, the $2^4 = 16$ points in the sample space are equally likely to occur.  therefore, the denominator is for all probabilities and also for our function it is 16.  in general, the event of selling x models with side airbags and $4 - x$ models without side airbags can occur in $\binom{4}{x}$ ways, where $x$ can be $0, 1, 2, 3,$ or $4$.  thus the probabability distribution $f(x) = P(X = x)$ is

$f(x) = \frac{1}{16}\binom{4}{x}$ for $x = 0, 1, 2, 3, 4$

$f(0) = \frac{\binom{4}{x}}{16} = \frac{1}{16}$

$f(1) = \frac{\binom{4}{x}}{16} = \frac{4}{16} = \frac{1}{4}$

$f(2) = \frac{\binom{4}{x}}{16} = \frac{6}{16} = \frac{3}{8}$

$f(3) = \frac{\binom{4}{x}}{16} = \frac{4}{16} = \frac{1}{4}$

$f(4) = \frac{\binom{4}{x}}{16} = \frac{1}{16}$

so the probability distribution is,

| x | 0 | 1 | 2 | 3 | 4 |
|:-:|:-:|:-:|:-:|:-:|:-:|
|**$f(x)$** | 1/16 | 1/4 | 3/8 | 1/4 | 1/16 |

### definition 3.5

**the cumulative distribution function** $F(x)$ of a discrete random variable $X$ with probability distribution $f(x)$ is

$$F(x) = P(X \leq x) = \sum_{t \leq x} f(t), \text{  for} -\infty \leq x \leq \infty$$

### example 3.10

find the cumulative distribution of the random variable $X$ in example 3.9 where $X$ is the number of cars with side airbags sold by the agency.

$$f(x) = \frac{1}{16}\binom{4}{x} , \text{  for  } x = 0, 1, 2, 3, 4$$ 

$f(0) = \frac{1}{16}$, $f(1) = \frac{1}{4}$, $f(2) = \frac{3}{8}$, $f(3) = \frac{1}{4}$, $f(4) = \frac{1}{16}$

$$F(0) = f(0) = \frac{1}{16}$$

### figure probability mass function plot


### figure probability histogram

### figure discrete cumulative distribution function

### continuous probability distributions

### joint probability distributions

## exercises

**3.5, 3.7 3.13, 3.14, 3.17, 3.33, 3.36, 3.38, 3.41, 3.43, 3.45, 3.47, 3.56**

3.5.  determine the value of c so that each of the following functions can serve as a probability distribution of the discrete random variable x.

a.  $f(x) = x(x^{2} + 4)$, for $x = 0, 1, 2, 3$

b.  $f(x) = c\binom{2}{x}\binom{3}{3-x}$, for $x = 0, 1, 2$

knowing that the summation of a pdf is 1 always we we get the following template

$$
1 = \sum_{x} f(x)
$$

, and substituting the given expression for $f(x)$ and simplifying, we get:

$$
1 = \sum_{x=0}^2 f(x) = f(0) + f(1) + f(2) = c\binom{2}{0}\binom{3}{3-0} + c\binom{2}{1}\binom{3}{3-1} + c\binom{2}{2}\binom{3}{3-2} = c(1)(1) + c(2)(3) + c(1)(3) = 5c
$$

$$5c = 1 \implies c = \frac{1}{5}$$

therefore, the value of $c$ that makes $f(x)$ a probability distribution is $c = \frac{1}{5}$.

3.7.  the total number of hours, measured in units of 100 hours, that a family runs a vacuum cleaner over a period of one year is a continuous random variable $X$ that has a probability density function.  

$$f(x) = 
\begin{cases}
x, 0 \eq x \eq 1, \\
2 - x, 1 \leq x \eq 2, \\
0, \text{otherwise} \\
\end{cases}
$$

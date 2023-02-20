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
- for a given sample space $S$ of some experiment, a random variable (rv) is any rule that associates a number with each outcome in $S$.

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
    - often this repressents count data, such as the number of defectives, highway fatalities, etc.

### continuous random variable

- **continuous random variable** if a random variable can take on values on a continuous scale
    - often represents measured data, such as heights, weights, temperatures, distance, or life periods

### definition 3.2 discrete sample space

**discrete sample space**  if a sample space contains a _finite number of possibilities_ or an unending sequence with as many elements as there are whole numbers.

### definition 3.3 continuous sample space

**continuous sample space** if a sample space contains an infinite number of possibilities equal to the number of points on a line segment.

### definition 3.4 probability mass function

### example 3.6

### example 3.8

### example 3.9

### definition 3.5

### example 3.10

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

Therefore, the value of $c$ that makes $f(x)$ a probability distribution is $c = \frac{1}{5}$.

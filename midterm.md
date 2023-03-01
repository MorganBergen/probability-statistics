# probability and stochastic processes

## statistics

1.  sample mean:  

$$\bar{x} = \sum_{i=1}^{n}\frac{x_{i}}{n} = \frac{x_{1} + x_{2} + \cdots + x_{n}}{n}$$

2.  sample median if $n$ is even:  $\tilde{x} = \frac{x_{\frac{n+1}{2}} + x_{\frac{n+2}{2}}}{2}$

3.  sample median if $n$ is odd $\tilde{x} = x_{\frac{n+1}{2}}$

4.  sample variance: $X_{1}, X_{2}, \cdots, X_{n}$ is denoted by $\sigma^{2}$

$$\sigma^{2} = s^{2} = \frac{1}{n - 1} \sum_{i=1}^{n} (x_{i} - \bar{x})^{2}$$

5.  sample standard deviation:  $s = \sqrt{s^{2}}$

## probability

0.  event operations:  
-  $A \cap \emptyset = \emptyset$
-  $A \cup \emptyset = A$
-  $A \cap A' = \emptyset$, $A \cup A' = S$
-  $S' = \emptyset$, $\emptyset' = S$
-  $(A \cap B)' = A' \cup B'$
-  $(A \cup B)' = A' \cap B'$

1.  $(A \cup B)^c = (A^c \cap B^c)$
2.  mutually exclusive events $A_{1}$ and $A_{2}$, $P[A_{1} \cup A_{2}] = P[A_{1}] + P[A_{2}]$

3.  if $A = A_{1} \cup A_{2} \cup \cdots \cup A_{m} \text{ and }  A_{i} \cap A_{j} = \emptyset \text { for all } i \neq j \text{ , then }$ $ P[A] = \sum_{i=1}^m P[A_{i}] $
4.  $P[.]$, $P[\emptyset] = 0$, $P[A^c] = 1 - P[A]$, $P[A \cup B] = P[A] + P[B] - P[A \cap B]$, and $A \subset B, P[A] \leq P[B]$

5.  $B = {s_{1}, s_{2}, \cdots, s_{m}}$ is the sum of the probabilities of the outcomes contained in the event:  $$ P[B] = \sum_{i=1}^m P[{s_{i}}] $$

6.  $S = {s_{1}, s_{2}, \cdots, s_{n}}$ in which each outcomes $s_{i}$ is equally likely, 

$$P[{s_{i}}] = \frac{1}{n}  \space \space \space  1 ≤ i ≤ n$$ 

7.  conditional probability measure $P[A|B]$

-  $P[A|B] \geq 0$
-  $P[B|B] = 1$
-  $A = A_{1} \cup A_{2} \cup \cdots \cup A_{m}$ and $A_{i} \cap A_{j} = \emptyset$ for all $i \neq j$, then, $P[A|B] = P[A_{1}|B] + P[A_{2}|B] + \cdots + P[A_{m}|B]$

8.  partition $B = B_{1}, B_{2}, \cdots, B_{m}$ and any event $A$ in the sample space, let $C_{i} = A \cap B_{i}$ For $i ≠ j$, the events $C_{i}$ and $C_{j}$ are mutually exclusive and $A = C_{1} \cup C_{2} \cup \cdots$

9.  $A$ and partition ${B_{1}, B_{2}, \cdots, B_{m}}$, 
$$P[A] = \sum_{i=1}^m P[A \cap B_{i}]$$

10.  law of total probability ${ B_{1}, B_{2}, \cdots, B_{m} }$ with $P[B_{i}] > 0$ for all $i$,

$$ P[A] = \sum_{i=1}^m P[A|B_i] P[B_i] $$

11.  conditional probability

$$
P(B | A) = \frac{P(A \cap B)}{P(A)} \\
\text{if } P(A) > 0 \\
$$

12.  bayes' theorem

$$
P(B_{r} | A) = \frac{P(B_{r} \cap A)}{\sum_{i = 1}^{k} P(B_{i} \cap A)} = \frac{P(B_{r} \cap A)}{\sum_{i = 1}^{k} P(B_{i} | A) P(B_{i})}
$$

$$ P[B|A] = \frac{P[A|B] P[B]}{P[A]} $$

13.  independent events two events $A$ and $B$ are independent if 

$$ P[AB] = P[A]P[B] $$

## 3. Discrete Random Variables

1.  **probability mass function** is the set of ordered pars $(x, f(x))$ is a probability function, probability mass function, or probability distribution of the discrete random variable $X$ if for each possible outcome $x$.

1.  $f(x) \geq 0$

2.  $\sum f(x) = 1$

3.  $P(X = x) = f(x)$

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

2.  **the cumulative distribution function** $F(x)$ of a discrete random variable $X$ with probability distribution $f(x)$ is

$$F(x) = P(X \leq x) = \sum_{t \leq x} f(t), \text{  for} -\infty \leq x \leq \infty$$

3.  continuous random variable has a probability of zero assuming exactly any of its values $P(a < X \leq b) = P(a < X < b) = P(a \leq X < b) = P(a \leq X \leq b)$

4.  the function $f(x)$ is a **probability density function** (pdf) for the continuous random variable $X$, defined over the set of real numbers, if 

1.  $f(x) \geq 0$ for all $x \in R$
2.  $\int_{-\infty}^{\infty} f(x) dx = 1$
3.  $P(a < X < b) = \int_{a}^{b} f(x) dx$

5.  definition of joint probability distribution / probability mass function  $f(x, y) = P(X = x, Y = y)$  the function $f(x, y)$ is a joint probability distribution or **probability mass function** of the discrete random variables $X$ and $Y$ if

1.  $f(x, y) \geq 0$ for all $(x, y)$

2.  $\sum_{x} \sum_{y} f(x, y) = 1$

3.  $P(X = x, Y = y) = f(x, y)$

for any region $A$ in the $xy$ plane, $P[(X, Y) \in A] = \sum_{}\sum_{A} f(x,y)$

## mathematical expectation

1.1. **expeted value**  let $X$ be a random variable with probability distribution $f(x)$, the **mean** or **expected value** of $X$ is

if $X$ is discrete 

$$\mu = E(X) = \sum_{x}{x f(x)}dx$$

if $X$ is continuous

$$\mu = E(X) = \int_{-∞}^{∞}{xf(x)}dx$$ 

4.1.  **example** a lot containing 7 components is sampled by a quality inspector; the lot contains 4 good components and 3 defective components. a sample of 3 is taken by the inspector. find the expected value of the number of good components in this sample.

let $X$ represent the number of good components in the sample.  the probability distribution of $X$ is 

$$f(x) = \frac{\binom{4}{x} \binom{3}{3 - x}}{\binom{7}{3}}, x = 0, 1, 2, 3$$

$f(0) = 1/35$,  $f(1) = 12/35$, $f(2) = 18/35$, $f(3) = 4/35$

$$\mu = E(X) = \sum_{x}{x f(x)}dx = (0) \frac{1}{35} + (1) \frac{12}{35} + (2) \frac{18}{35} + (3) \frac{4}{35} = 1.7$$

therefore if a sample size 3 is selected at random over and over again from a lot of 4 good components and 3 defective components, it will contain on average 1.7 good components

4.4.  **example** a coin is biased such that a head is three times as likely to occur as a tail. Find the expected number of tails when this coin is tossed twice.

assigning weights of $3w$ and $w$ for a head and tail respectively.  we obtain $P(H) = 3/4$ and $P(T) = 1/4$.  the sample space for the experiment is $S = \{HH, HT, TH, TT\}$.  now if $X$ represents the number of trials that occur in two tosses of coins, we have

$P(X = 0) = P(HH) = (3/4)(3/4) = 9/16$

$P(X = 1) = P(HT) + P(TH) = (3/4)(1/4) + (1/4)(3/4) = 3/8$

$P(X = 2) = P(TT) = (1/4)(1/4) = 1/16$

the probability distribution for $X$ is then

| x | 0 | 1 | 2 |
|:-:|:-:|:-:|:-:|
|$f(x)$| 9/16 | 3/8 | 1/16 |

**expected value** is $\mu = E(X) = (0)(9/16) + (1)(3/8) + (2)(1/16) = 1/2$ 

1.2. **expected value**  let $X$ and $Y$ be random variables with joint probability distribution $f(x, y)$.  the mean or expected value of the random variable $g(X, Y)$ is

if $X$ and $Y$ are discrete

$$\mu_{g(X, Y)} = E[g(X, Y)] = \sum_{x} \sum_{y} g(x, y) f(x, y)$$

if $X$ and $Y$ are continuous

$$\mu_{g(X, Y)} = E[g(X, Y)] = \int_{-\infin}^{\infin}\int_{-\infin}^{\infin} g(x, y) f(x, y) dx dy$$

1.3.  **standard deviation**  let $X$ be a random variable with probability distribution $f(x)$ and mean $\mu$.  the variance of $X$ is $\sigma^{2}$.  the variance $\sigma^{2}$ is called the standard deviation.

if $X$ is discrete
$$
\sigma^{2} = E[(X - \mu)^{2}] = \sum_{x} (x - \mu)^{2} f(x)dx
$$

if $X$ is continuous
$$
\sigma^{2} = E[(X - \mu)^{2}] = \int_{-\infin}^{\infin} (x - \mu)^{2} f(x) ds
$$

1.4.  the variance of the random variable $X$ is $\sigma^{2} = E(X^{2}) - \mu^{2}$

1.5.  let $X$ be a random variable with probability distribution $f(x)$ the variance of the random variable $g(X)$ is

if $X$ is discrete

$$\sigma_{g(X)}^{2} = E\{[g(X) - \mu_{g(X)}^{2}\} = \sum_{x} [g(x) - \mu_{g(X)}]^{2} f(x)$$

if $X$ is continuous

$$\sigma_{g(X)}^{2} = E\{[g(X) - \mu_{g(X)}]^{2}\} = \int_{-\infin}^{\infin} [g(x) - \mu_{g(X)}]^{2}f(x) dx$$

1.6.  **covariance** let $X$ and $Y$ be random variables with joint probability distribution $f(x, y)$ the covariance of $X$ and $Y$ is 
if $X$ and $Y$ are discrete

$$ \sigma_{XY} = E[(X - \mu_{X})(Y - \mu_{Y})] = \sum_{x} \ sum_{y} (x - \mu_{X})(y - \mu_{y}) f(x, y)$$

if $X$ and $Y$ are continuous 

$$ \sigma_{XY} = E[(X - \mu_{X})(Y - \mu_{Y})] =  \int_{-\infin}^{\infin}\int_{-\infin}^{\infin}(x - \mu_{X})(y - \mu_{y}) f(x, y) dx dy$$

1.5. **covariance** the covariance of two random variables $X$ and $Y$ with means/expected valyes of $\mu_{X}$ and $\mu_{Y}$ is $\sigma_{XY} = E(XY) - \mu_{X}\mu_{Y}$

4.13  **example** there are a number of blue refills $X$ and the number of red refills $Y$.  two refills for a ballpoint pen are selected at random from a certain box, and the following is the joint probability distribution


| f(x, y) | x = 1 | x = 1 | x = 2 | h(y) |
|:-------:|:-----:|:-----:|:-----:|:----:|
|y = 0    | 3/28  | 9/28  | 3/28  | 5/28 |
|y = 1    | 3/14  | 3/14  | 0     | 3/7  |
|y = 2    | 1/28  | 0     | 0     | 1/28 |
|**g(x)** | 5/14  | 14/28 | 3/28  | 1    |

find the covariance of $X$ and $Y$  the expected value E(XY) is = 3/14

$$E(XY) = \sum_{x = 0}^{2} \sum_{y = 0}^{2} xy f(x, y) = (0)(0)f(0, 0) = (0)(1)f(0, 1) + (1)(0)f(1, 0) + (1)(1) f(1, 1) + (2)(0)f(2, 0)$$

$$E(XY) = f(1, 1) = 3/14$$

now the covariance is therefore,

$$\mu_{X} = \sum_{x = 0}^{2} x g(x) = (0)(5/14) + (1)(15/28) + (2)(3/28) = 3/4$$

$$\mu_{Y} = \sum_{y = 0}^{2} y h(y) = (0)(15/28) + (1)(3/7) + (2)(1/28) = 1/2$$

$$\sigma_{XY} = E(XY) - \mu_{X} \mu_{Y} = (3/14) - (3/4)(1/2) = -9/56$$

4.14 **example**  the fraction $X$ of male runners anfd the fraction $Y$ of feamle runners who compete in marathon races are described by the joint density function, find the covariance of $X$ and $Y$

$$
f(x, y) = 
\begin{cases}
8xy, & 0 \leq y \leq x \leq 1 \\
0, & \text{ elsewhere} \\
\end{cases}
$$

first we compute the marginal density function, they are

$$
g(x) = 
\begin{cases}
4x^{3}, & 0 \leq x \leq 1, \\
0, & \text{ elsewhere} , \\
\end{cases}
$$

$$
h(x) = 
\begin{cases}
4y(1 - y^{2}), & 0 \leq x \leq 1, \\
0, & \text{ elsewhere} , \\
\end{cases}
$$

then we compuete the joint density function

$$
\mu_{X} = E(X) = \int_{0}^{1}\int_{y}{1} 8x^{2} y^{2} dx dy = 4/9
$$

$$
\sigma_{XY} = E(XY) - \mu_{X}\mu{Y} = 4/9 - (4/5) (8/15) = 4/225
$$

1.6.  **correlation coefficient** of $X$ and $Y$, let $X$ and $Y$ be random variables with covariance $\sigma_{XY}$ and standard deviation $\sigma_{X}$ and $\sigma_{Y}$, the correlation coefficient of $X$ and $Y$

$$ \rho_{XY} = \frac{\sigma_{XY}}{\sigma_{X} \sigma_{Y}}$$

4.15.  **example**  find the correlation coefficient between X and Y in example 4.13  

$$E(X^{2}) = (0^{2})(5/14) + (1^{2})(15/28) + (2^{2})(3/28) = 27/28$$

$$E(X^{2}) = (0^{2})(15/28) + (1^{2})(3/7) + (2^{2})(1/28) = 4/7$$

$$\sigma_{X}^{2} = 27/28 - (3/4)^{2} = 45/112$$

$$\sigma_{Y}^{2} = 4/7 - (1/2)^{2} = 9/28$$

therefore the correlation coefficient between $X$ and $Y$ are

$$\rho_{XY} = \frac{\sigma_{XY}}{\sigma_{X}\sigma_{Y}} = \frac{-9/56}{\sqrt{(45/112)(9/28}} = -\frac{1}{\sqrt{5}}$$

4.16 **example** find the correlation coefficient of $X$ and $Y$ in example 4.14, because 

$$E(X^{2}) = \int_{0}^{1} 4x^{5}dx = \frac{2}{3}$$

$$E(Y^{2}) = \int_{0}^{1} 4y^{3}(1-y^{2})dy = 1 - \frac{2}{3} = \frac{1}{3}$$

$$\rho_{XY} = \frac{2/225}{\sqrt{(2/75)(11/225)}} = \frac{4}{\sqrt{66}}$$

4.34.  **exercise**  let $X$ be a random variable with the following probability distribution

| **X** | -2 | 3  | 5  | 
|:-----:|:--:|:--:|:--:|
|**$f(x)$**| 0.3 | 0.2 | 0.5 |

find the standard deviation of $X$

$\mu = (-2)(f(-2)) + (3)(f(3)) + (5)(f(5))$

$\mu = (-2)(0.3) + (3)(0.2) + (5)(0.5)$

$E(X^{2}) = (0)^{2}(0.4) + (1)^{2}(0.3) + (2)^{2}(0.2) + (3)^{2}(0.1) = 2.0$

$\sigma_{2} = E(X^{2}) - \mu^{2} = 9.25$ and $\sigma = 3.041$


























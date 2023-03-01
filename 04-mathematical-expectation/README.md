#  mathematical expectation

you will be asked to find the correlation coefficient in the exam
you will be ased in 4.14 and 4.16

**contents**

1.  [mean and variance of a random variable](#mean-and-variance-of-a-random-variable)
2.  [covariance of two random variables](#covariance-of-two-random-variable)
3.  [means and variances of linear combinations of random variables](#means-and-variances-of-linear-combinations-of-random-variables)
4.  [chebyshev's theorem](#chebyshev's-theorem)

##  mean and variance of a random variable

1.  mean of the random variable

in chapter 1 we discussed the sample mean, which is the arithmetic mean of the data.  now consider the following.  if two coins are tossed 16 times and $X$ is the number of heads that occur per toss, then the values of $X$ are 0, 1, and 2.  suppose that the experiment yields no heads, one head and two heads a total of 4, 7, and 5 times respectively.  the average number of heads per toss of the two coins is then 

-  2 coins tossed 16 times
-  $X$ is the number of heads that occur per toss: $X \in \{0, 1, 2\}$
-  outcome of experiment $0$ heads $4$ times, $1$ head $7$ times, $2$ heads $5$ times in total.

$$
\frac{(0 \times 4) + (1 \times 7) + (2 \times 5)}{16} = 1.125
$$

this is the average value of the data and yet to is not a possible outcome of $\{0, 1, 2\}$.  hence, the average is not necessarily a possible outcome for the experiment.  for instance, a salesman's average monthly income is not likely to be equal to any of his monthly paychecks.  lets now restructure our computation for the average number of heads so as to have the following equivalent form.

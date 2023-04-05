# midterm 2 

###  contents
1.  [5.25](#525)
2.  [5.27](#527)
3.  [5.66](#566)
4.  [5.67](#567)
1.  [5.3 example](#53-example)
5.  [6.8](#68)
6.  [6.32](#632)
7.  [6.34](#632)
8.  [6.55](#655)
9.  [6.66](#666)
10. [8.27](#827)
11. [8.30](#830)
12. [central limit theorem and its conditions](#central-limit-theorem-and-its-conditions)

###  examples

2.  [6.17 example](#617-example)
3.  [6.20 example](#620-example)

### 5.25

**question** suppose that for a very large shipment of integrated-circuit chips, the probability of failure for any one chip 0.10.  assuming that the assumptions underlying the binomial distributions are met, find the probability that at most 3 chips fail in a random sample of 20.

**solution**  let random variable $X$ represent the number of chips failed among the 20 randomly selected chips.  we will consider failure of a chip as a success.  thus the probability of success is $p = 0.10$ and because the trails are independent, $X$ has a binomial distribution with parameters $n = 20$ and $p = 0.10$.  the probability mass function of $X$ is, 

$$P(X = x) = b(x; 20, 0.10), \text{    } x = 0, 1, 2, \dots, 20$$

$$\binom{20}{x} (0.10)^{x}(1 - 0.10)^{20 - x}= \binom{6}{x} (0.10)^{x}(0.90)^{20 - x}, \text{   } x = 0, 1, 2, \dots, 20$$

now to find the probability that at most $3$ chips fail in a random sample of $20$

$$P(X \leq 3) = \sum_{x = 0}^{3} b (x; 20, 0.10) = 0.8670$$


###  5.27

**question** if the probability that a fluorescent light has a useful life of at least 800 hours in 0.9, find the probabilities that among 20 such lights

**solution**  let random variable $X$ represent the number of lights having a useful life of at least 800 hours among 20 lights.  lets consider it success if a light has a useful life of at least 800 hours.  thus, the probability of a success in each trial is $p = 0.90$.  because the trials are independent $X$ has a binomial distribution with parameters $n = 20$ and $p = 0.90$.  the probability mass function of $X$ is,

$$P(X = x) = b(x; 20, 0.90), x = 0, 1, 2, \dots , 20$$

$$= \binom{20}{x}(0.90)^{x}(1 - 0.90)^{20 - x} = \binom{20}{x}(0.90)^{x}(0.10)^{20 - x}, x = 0, 1, 2, \dots, 20$$

a.  exactly 18 will have a useful life of at least 800 hours

$$P(X = 18) = b(18; 20, 0.90) = \binom{20}{18}(0.90)^{18}(0.10)^{20 - 18} = \frac{20!}{18! 2!}(0.90)^{18}(0.10)^{2} = 0.2852$$

b.  at least 15 will have a useful life of at least 800 hours

$$P(X \geq 15) = 1 - P(X \leq 14) = 1 - \sum_{x = 0}^{14}b(x; 20, 0.90) = 1 - 0.0113 = 0.9887$$

c.  at least 2 will not have a useful life of at least 800 hours

because the total number of lights is 20 the event that at least 2 will not have a useful life of at least 800 hours can be looked as at most 18 will have a useful life of at least 800 hours therefore using the table a1 from the appendex we get,

$$P(X \leq 18) = \sum_{x = 0}^{18} b(x; 20, 0.90) = 0.608$$

###  5.66

**question** changes in airport procedures require considerable planning.  arrival rates of aircraft are important factors that must be taken into account.  suppose small aircraft arrive at a certain airport, according to a poisson process, at the rate of 6 per hour.  thus the poisson parameter for arrivals over a period of hours is $\mu = 6t$ 

**solution**  let random variables $X$ represent the number of aircraft arrivals during a one hour period.  the poisson parameter for arrivals for a period of $t$ hours is $\mu = 6t$.  the probability mass function of $X$ is 

a.  what is the probability that exavctly 4 small aircraft arrive during a 1-hour period?

$P(X = x) = \frac{e^{-6}(6)^{4}}{4!} = 0.1339$

b.  what is the probability that at least 4 arrive during a 1-hour period?

$P(X \geq 4) = 1 - P(X \leq 3) = 1 - P(X \leq 3) = 1 - P(X = 0) - P(X = 1) - P(X = 2) - P(X = 3)$

$=1 - p(0;6) - p(1;6) - p(2;6) - p(3;6)$

$= 1 - \frac{e^{-6}(6)^{0}}{0!} - \frac{{e^{-6}(6)^{1}}}{1!} - \frac{{e^{-6}(6)^{2}}}{2!} - \frac{e^{-6}(6)^{3}}{3!}$

$= 1 - 0.002479 - 0.014873 - 0.044618 - 0.089235$

$= 1 - 0.151204 = 0.8488$

c.  if we define a working day as 12 hours, what is the probability that at least 75 small aircraft arrive during a working day?

$t = 12 \text{ hours} \implies \mu = 6t = 6 \times 12 = 72 \text{ hours}$

$P(X \geq 75) = 1 - P(X \leq 74) = 1 - \sum_{x = 0}^{74} \frac{e^{-72}(72)^{x}}{x!} = 1 - 0.6227 = 0.3773$

###  5.67

the number of customers arriving per hour at a certain automobile service facility is assumed to follow a poisson distribution with mean $\lambda = 7$

the number of customers arriving per hours follow the poisson distribution with mean $\lambda = 7$, therefore arrival rate of customers is 7 per hour.  let random variable $X$ represent the number of arrivals of customers in 2 hour, therefore $t = 2$.  $X$ has a poisson distribution with parameter $\mu = 7 \times 2 = 14$.  therefore the probability mass function of $X$ is,

$P(X = x) = p(x; \mu), \text{ where } x = 0, 1, 2, 3, \dots$ 

$= e^{-\mu}\frac{(\mu)^{x}}{x!} = e^{-14}\frac{(14)^{x}}{x!}$

a.  compute the probability that more than 10 customers will arive in a 2-hour period

$P(X > 10) = 1 0 P(X \leq 10) = 1 - \sum_{x = 0}^{10}p(x; 14) = 1 - 0.175681 = 0.8243$

b.  what is the mean number of arrivals during a 2-hour period?

$X$ has a poisson distribution with parameter $\mu = 7 \times 2 = 14$.  the mean of random variable with poisson distribution with parameter $\mu$ is $E(X) = \mu$.  therefore the mean number of arrivals in 2 hours in $E(X) = 14$

###  5.3 example


**example 5.3**  a large chain retailer purchases a certain kind of electronic device from a manufacturer.  the manufacturer indicates that defective rate of the device is $3\%$.

a.  the inspector of the retailer randomly picks 20 items from a shipment.  what is the probability that there will be at least one defective item among these 20?

denote by $X$ the number of defective devices among the 20; $b(x; 20, 0.03)$

$$P(X \geq 1) = 1 - P(X = 0) = 1 - b(0; 20, 0.03) = (1 - 0.03^{0})(0.97^{20 - 0}) = 0.4562$$

b.  suppose that the retailer receives 10 shipments in a month and the inspector randomly tests 20 devices per shipment.  what is the probability that there will be 3 shipments containing at least one defective device?

denote by $Y$ the number of shipments containing at least one defective item $b(y; 10, 0.4562)$

$$P(Y = 3) = {{10}\choose{3}} 0.4562^{3}(1 - 0.4562)^{10 - 3} = 0.1602$$

###  6.8

given a normal distribution with $\mu = 30$ and $\sigma = 6$, find

a.  the normal curve area to the right of $x = 17$

$$z = \frac{x - \mu}{\sigma} = \frac{17 - 30}{6.0} \approx -2.17$$

$\therefore P(X > 17) = P(Z > -2.17) = 1 - P(Z \leq -2.17) = 1 - 0.0150 = 0.9850$

b.  the normal curve area to the left of $x = 22$

$$z = \frac{x - \mu}{\sigma} = \frac{22 - 30}{6.0} \approx -1.33$$

$$\therefore P(X < 22) = P(Z < -1.33) = 0.0918$$

c.  the normal curve area between $x = 32$ and $x = 41$

$$z_{1} = \frac{x_{1} - \mu}{\sigma} = \frac{32 - 30}{6.0} \approx 0.33$$

$$z_{2} = \frac{x_{2} - \mu}{\sigma} = \frac{41 - 30}{6.0} \approx 1.83$$

$$\implies P(32 < X < 41) = P(X < 41) - P(X < 32)$$

$$= P(Z_{2} < 1.83) - P(Z_{1} < 0.33) = 0.9664 - 0.6293 = 0.3371$$ 

d.  the value of $x$ that has $80\%$ of the normal curve area to the left

$$z = \frac{x - \mu}{\sigma}$$

$$x = {\sigma}z + \mu = 6 \cdot 0.842 + 30 = 35.05$$

e.  the tow values of $x$ rthat conatin the middle $75\%$ of the normal curve area

$P(-z \leq Z \leq z) = 0.75$

$P(Z \leq z) - P(Z \leq -z) = 0.75$

$P(Z \leq z) - (1 - P(Z \leq z)) = 0.75$

$2 P(Z \leq z) - 1 = 0.75$

$2 P(Z \leq z) = 0.75$

$P(Z \leq z) = 0.875$

therefore the value of $z$ that leaves an area of 0.875 to the right is $z_{1} = -1.15$ and the left is $z_{2} = 1.15$

$$z_{1} = \frac{x_{1} - \mu}{\sigma}$$


###  6.32

a pharmaceutical company knows that approximately $5\%$ of its birth-control pulls have an ingredient that is below the minimum strength, thus rendering the pill ineffective.  what is the probability that fewer than 10 in a sample of 200 pills will be ineffective?

-  the total number of pills is $n = 200$
-  we consider it a success if a pill is ineffective
-  the probability of a success in each trial is $p = 5\% = \frac{5}{100} = 0.5$
-  therefore the probability of failure is $q = 1 - p = 1 - 0.5 = 0.95$
-  let the random variable $X$ represent the number of ineffective pills in a sample of 200 pills
-  therefore $X$ has a binomial distribution with parameters $n = 200$ and $p = 0.05$
-  the mean of binomial distribution is 
    -  $\mu = np \implies \mu = 200 \cdot 0.05 = 10$
-  the standard deviation of binomial distribution is
    -  $\sigma = \sqrt{npq} \implies \sqrt{200 \cdot 0.05 \cdot 0.95} = \sqrt{9.5} = 3.082$
-  to calculate the prob that fewer than 10 in a sample of 200 pills will be effective, or in otherworse we need to find the area to the left of $x = 9.5$
    -  $z = \frac{x - \mu}{\sigma} = \frac{9.5 - 10}{3.082} = -0.16$
    -  $\therefore P(X < 10) = P(Z < -0.16) \implies P(X < 10) = 0.4364$

###  6.34

a pair of dice is rolled 180 times.  what is the probability that a total of 7 occurs

-  the total number of trails ia $n = 180$
-  we consider it success if when rolling a pair of dice a total of 7 occur
-  the number favorable case to get the total of 7 is (1, 6), (2, 5), (3, 4), (4, 3), (5, 2), (6, 1) = 6
-  the total number of cases wqhen rolling a pair of dice is $6 \cdot 6 = 36$
-  the prob of a success in each trial is $p \frac{6}{36} = 0.1667$
-  therefore the probability of failure is $q = 1 - p = 1 - 0.1667 = 0.8333$
-  let random variable $X$ represent the number of successes among 180 trials
-  therefore $X$ has a binomial distribution with parameters $n = 180$ and $p = 0.1667$
-  the mean of binomial distribution is $\mu = np \implies \mu = 180 \cdot 0.1667 = 30$
-  the standard deviation fo binomial distribution is $\sigma = \sqrt{npq} = \sqrt{180 \cdot 0.1667 \cdot 0.8333} = \sqrt{25} = 5$

a.  at least 25 times?

-  the probability that 7 occur at least 25 times, mean that we need to find the area to the right of $x = 24.5$
-  $z = \frac{x - \mu}{\sigma} = \frac{24.5 - 30}{5} = -1.1$
-  $\therefore P(X \geq 25) = P(Z \geq -1.1) = 1 - P(Z < 1.1) = 1 - 0.1357 = 0.8643$

b.  between 33 and 41 times inclusive?

-  we have to now find the area between $x_{1} = 32.5$ and $x_{2} = 41.5$
-  $z_{1} = \frac{x_{1} - \mu}{\sigma} = \frac{32.5 - 30}{5} = 0.5$
-  $z_{2} = \frac{x_{2} - \mu}{\sigma} = \frac{41.5 - 30}{5} = 2.3$
-  $\therefore P(33 \leq X \leq 41) = P(0.05 < Z < 2.30) = P(Z < 2.30) - P(Z < 0.50) = 0.9893 - 0.6915 = 0.2978$

c.  exactly 30 times?

-  we have to find the area under the curve that is between $x_{1} = 29.5$ and $x_{2} = 30.5$
-  $z_{1} = \frac{x_{1} - \mu}{\sigma} = \frac{29.5 - 30}{5} = -0,1$
-  $z_{2} = \frac{x_{2} - \mu}{\sigma} = \frac{30.5 - 30}{5} = 0.1$
-  $\therefore P(X = 30) = P(-0.10 \leq Z \leq 0.10) = P(Z \leq 0.10) - P(Z \leq -0.10) = 0.5398 - 0.4602 = 0.0796$

###  6.55

computer response time is an important application of the gamma and exponential distributions.  suppose that a study of a certain computer system reveals that the response time, in seconds, has an exponential distribution with mean of 3 seconds.

a.  what is the probability that response time exceeds 5 seconds?

-  let the random variable $X$ represent the response time, in seconds
-  $X$ has an exponential distribution with a mean of $\beta = 3 \text{ seconds }$
-  the probability density function of exponential distribution is,
-  $f(x; \beta) = \frac{1}{3} e^{-x/\beta} \implies f(x; 3) = \frac{1}{3} e^{-x/3} ; x \geq 0$ 
-  $P(X > 5) = 1 - P(X \leq 5) = 1 - \frac{1}{3} \int_{0}^{5} e^{-x/3} dx = 1 - (1 - e^{-5/3}) = e^{-5/3} = 0.1889$

b.  what is the probability that response time exceeds 10 seconds?

-  $P(X > 10) = 1 - P(X \leq 10) = 1 - \frac{1}{3} \int_{0}^{10} e^{-x/3} dx = 1 - (1 - e^{10/3}) = e^{-10/3} = 0.0357$

###  6.66

a certain type of device has an advertised failure rate of 0.01 per hour.  the failure rate is constant and the exponential distribution applies.

a.  what is the mean time of failure?

-  an advertised failure rate of $\lambda = 0.01$%
-  let random variable $X$ represent the fialure rate of a certain type of device
-  therefore $X$ follows the exponential distribution with parameter $\lambda = 0.01$
-  the mean time to failure is thus, $\mu = \frac{1}{\lambda} = \frac{1}{0.01} = 100$

b.  what is the probability that 200 hours will pass before a failure is observed?

-  $P(X \leq 200) = 100 - P(X \leq 200) = 1 - (1 - e^{-0.01 \times 200}) = e^{-0.01 \times 200} = 0.1353$

###  8.27

in a chemical process, the amount of a certain type of impurity in the output is difficult to control and is thus a random variable.  speculation is that the population mean amount of the impurity is $0.20$ gram per gram of output.  it is known that the standard deviation is $0.1$ gram per gram.  an experiment is conducted to gain more insight regarding the speculation that $\mu = 0.2$.  the process is run on a lab scale $50$ times and the sample average $\bar{x}$ turns out to be $0.23$ gram per gram.  comment on the speculation that the mean amount of impurity is $0.20$ gram per gram.  make use of the central limit theorem in your work.

###  8.30

the mean score for freshman on an aptitude test at a certain college is $540$ with a standard deviation of $50$.  assume the means to be measured to any degree of accuracy.  what is the probability that two groups selected at random, consisting of $32$ and $50$ students, respectively will differ in their mean scores by

a.  more than 20 points

b.  an amount between $5$ and $10$ points?




<br><br><br><br><br><br><br><br><br><br><br><br><br><br>

###  6.17 example

**question**

suppose that a system contains a certain type of component whose time, in years, to failure is given by $T$.  the raindom variable $T$ is modeled nicely by the exponential distribution with mean time to failure $\beta = 5$.  if 5 of these components are installed in different systems, what is the probability that at least 2 are still functioning at the end of 8 years?

**solution**

the probability that a given component is still functioning after 8 years is given by

$$
P(T > 8) = \frac{1}{5}\int_{8}^{\infty} e^{-t/5} dt = e^{-8/5} \approx 0.2
$$

let X represent the number of components functioning after 8 years.  then using the binomial distribution, we have

$$
P(X \geq 2) = \sum_{x = 2}^{5} b(x; 5, 0.2) = 1 - \sum_{x = 0}^{1} b(x; 5, 0.2) = 1 - 0.7373 = 0.2627
$$

###  6.20 example

**question** &nbsp; &nbsp; it is known from pervious data, that the length of time in months between customer complaints about a certain product is a gamma distribution with $\alpha = 2$ and $\beta = 4$.  changes were made to tighten quality control requirements.  following these changes, 20 months passed before the first complaint.  does it appear as if the quality control tightening was effective?

**solution** &nbsp; &nbsp; let $X$ be the time to the first complaint, which, under conditions prior to the changes, followed a gamma distribution with $\alpha = 2$ and $\beta = 4$.  the question centers around how rare $X \geq 20$ is, given that $\alpha$ and $\beta$ remain at values $2$ and $4$, respectively.  in other words, under the prior conditions is a "time to complaint" as large as 20 months reasonable?  thus

$$
P(X \geq 20) = 1 - \frac{1}{\beta^{\alpha}} \int_{0}^{20} \frac{x^{\alpha - 1}e^{-x/\beta}}{\Gamma(\alpha)} 
$$

using $y = x/\beta$ we have

$$
P(X \geq  20) = 1 - \int_{0}^{5} \frac{ye^{-y}}{\Gamma(2)}dy = 1 - F(5; 2) = 1 - 0.96 = 0.04
$$

where $F(5; 2) = 0.96$ is found from table a.23.  as a result we could conclude that the conditions of the gamma distribution with $\alpha = 2$ and $\beta = 4$ are not supported by the data that an observed time to complaint is as large as $20$ months.  thus, it is reasonable to conclude that the quality control work was effective.

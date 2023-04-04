# midterm 2 

###  contents
1.  [5.25](#525)
2.  [5.27](#527)
3.  [5.66](#566)
4.  [5.67](#567)
5.  [6.8](#68)
6.  [6.32](#632)
7.  [6.34](#632)
8.  [6.55](#655)
9.  [6.66](#666)
10. [8.27](#827)
11. [8.30](#830)
12. [central limit theorem and its conditions](#central-limit-theorem-and-its-conditions)

###  examples

1.  [5.3 example](#53-example)
2.  [6.17 example](#617-example)
3.  [6.20 example](#620-example)

### 5.25

**question** suppose that for a very large shipment of integrated-circuit chips, the probability of failure for any one chip 0.10.  assuming that the assumptions underlying the binomial distributions are met, find the probability that at most 3 chips fail in a random sample of 20.

**solution**  let random variable $X$ represent the number of chips failed among the 20 randomly selected chips.  we will consider failure of a chip as a success.  thus the probability of success is $p = 0.10$ and because the trails are independent, $X$ has a binomial distribution with parameters $n = 20$ and $p = 0.10$.  the probability mass function of $X$ is, $P(X = x) = b(x; 20, 0.10), \text{    } x = 0, 1, 2, \dots, 20$

$$b(x; 20, 0.1)= \binom{20}{x} (0.10)^{x}(1 - 0.10)^{20 - x}$$

$= \binom{6}{x} (0.10)^{x}(0.90)^{20 - x}, \text{   } x = 0, 1, 2, \dots, 20$

now to find the probability that at most $3$ chips fail in a random sample of $20$

$$P(X \leq 3) = \sum_{x = 0}^{3} b (x; 20, 0.10) = 0.8670$$


###  5.27

question** if the probability that a fluorescent light has a useful life of at least 800 hours in 0.9, find the probabilities that among 20 such lights

a.  exactly 18 will have a useful life of at least 800 hours

b.  at least 15 will have a useful life of at least 800 hours

c.  at least 2 will not have a useful life of at least 800 hours

###  5.66

changes in airport procedures require considerable planning.  arrival rates of aircraft are important factors that must be taken into account.  suppose small aircraft arrive at a certain airport, according to a poisson process, at the rate of 6 per hour.  thus the poisson parameter for arrivals over a period of hours is $\mu = 6t$ 

a.  what is the probability that exavctly 4 small aircraft arrive during a 1-hour period?

b.  what is the probability that at least 4 arrive during a 1-hour period?

c.  if we define  aworking day as 12 hours, what is the probability that at least 75 small aircraft arrive during a working day?

###  5.67

the number of customers arriving per hour at a certain automobile service facility is assumed to follow a poisson distribution with mean $\lambda = 7$

a.  compute the probability that more than 10 customers will arive in a 2-hour period

b.  what is the mean number of arrivals during a 2-hour period?

###  6.8

given a normal distribution with $\mu = 30$ and $\sigma = 6$, find

a.  the normal curve area to the right of $x = 17$

b.  the normal curve area to the left of $x = 22$

c.  the normal curve area between $x = 32$ and $x = 41$

d.  the value of $x$ that has $80\%$ of the normal curve area to the left

e.  the tow values of $x$ rthat conatin the middle $75\%$ of the normal curve area

###  6.32

a pharmaceutical company knows that approximately $5\%$ of its birth-control pulls have an ingredient that is below the minimum strength, thus rendering the pill ineffective.  what is the probability that fewer than 10 in a sample of 200 pills will be ineffective?

###  6.34

a pair of dice is rolled 180 times.  what is the probability that a total of 7 occurs

a.  at least 25 times?

b.  between 33 and 41 times inclusive?

c.  exactly 30 times?

###  6.55

computer response time is an important application of the gamma and exponential distributions.  suppose that a study of a certain computer system reveals that the response time, in seconds, has an exponential distribution with mean of 3 seconds.

a.  what is the probability that response time exceeds 5 seconds?

b.  what is the probability that response time exceeds 10 seconds?

###  6.66

a certain type of device has an advertised failure rate of 0.01 per hour.  the failure rate is constant and the exponential distribution applies.

a.  what is the mean time of failure?

b.  what is the probability that 200 hours will pass before a failure is observed?


###  8.27

in a chemical process, the amount of a certain type of impurity in the output is difficult to control and is thus a random variable.  speculation is that the population mean amount of the impurity is $0.20$ gram per gram of output.  it is known that the standard deviation is $0.1$ gram per gram.  an experiment is conducted to gain more insight regarding the speculation that $\mu = 0.2$.  the process is run on a lab scale $50$ times and the sample average $\bar{x}$ turns out to be $0.23$ gram per gram.  comment on the speculation that the mean amount of impurity is $0.20$ gram per gram.  make use of the central limit theorem in your work.

###  8.30

the mean score for freshman on an aptitude test at a certain college is $540$ with a standard deviation of $50$.  assume the means to be measured to any degree of accuracy.  what is the probability that two groups selected at random, consisting of $32$ and $50$ students, respectively will differ in their mean scores by

a.  more than 20 points

b.  an amount between $5$ and $10$ points?




<br><br><br><br><br><br><br><br><br><br><br><br><br><br>

###  5.3 example


**example 5.3**  a large chain retailer purchases a certain kind of electronic device from a manufacturer.  the manufacturer indicates that defective rate of the device is $3\%$.

a.  the inspector of the retailer randomly picks 20 items from a shipment.  what is the probability that there will be at least one defective item among these 20?

denote by $X$ the number of defective devices among the 20; $b(x; 20, 0.03)$

$$P(X \geq 1) = 1 - P(X = 0) = 1 - b(0; 20, 0.03) = (1 - 0.03^{0})(0.97^{20 - 0}) = 0.4562$$

b.  suppose that the retailer receives 10 shipments in a month and the inspector randomly tests 20 devices per shipment.  what is the probability that there will be 3 shipments containing at least one defective device?

denote by $Y$ the number of shipments containing at least one defective item $b(y; 10, 0.4562)$

$$P(Y = 3) = {{10}\choose{3}} 0.4562^{3}(1 - 0.4562)^{10 - 3} = 0.1602$$

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

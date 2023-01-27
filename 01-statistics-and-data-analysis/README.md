# ch 01 introduction to statistics and data analysis

**contents**

1.  [what is statistics](#what-is-statistics)
2.  [inferential statistics](#inferential-statistics)
3.  [descriptive statistics](#descriptive-statistics)
4.  [role of probability](#role-of-probability)
5.  [data collection and sampling procedures](#data-collection-and-sampling-procedures)
6.  [pictorial and tabular methods in descriptive statistics](#pictorial-and-tabular-methods-in-descriptive-statistics)
7.  [measures of location](#measures-of-location)
8.  [measures of variability](#measures-of-variability)
9.  [discrete and continuous data](#discrete-and-continuous-data)
10. [general types of statistical studies](#general-types-of-statistical-studies)

## what is statistics

- statistics is a way to get information from data
- statistics means numerical descriptions to most people
- statistics is a discipline which is concerned with:
    - designing experiements and data collection
    - summarizing information to aid understanding
    - analyzing and drawing conclusions from data
    - estmating the present or predicting the future
- in making predictions, statistics used the companion subject of probability, which models chance mathematically and enables calculations of change in complicated cases

## inferential statistics

- inferential statistics are the mathematical procedures hereby we convert information about the sample into intelligent guesses about the population

- it utilizes sample data to make estimates, decisions, predictions, or other generalizations about larger set of data

- this is also called inductive reasoning or inductive statistics
    - deduction - from the general facts to partiulcar cases:  mathematics
    - induction - from a particular case to a general one:  statistics

## descriptive statistics

- descriptive statistics consists of methods for organizing displaying, and describing data to convey information by using tables, graphs, and summary measure
- descriptive statistics are just descriptive. they do not involve generalizing beyond the data at hand.
- it utilizes graphical and numerical methods to look at patterns, to summarize, and to present the information in a set of data
- other involve calculation of numerical summary measures such as mean, standard deviation, and correlation coefficients
- software:  calcular, r, sas, spss, stata,...
- with descriptive statistics, we are simply describing what the data shows
- with inferential statsitics, we are trying to make inferences from our data to more general conditions

## role of probability

- for a statistical problem, the sample along with inferential statistics allow us to draw conclusions about the population, with inferential statistics making clear use of elements of probability. (inductive in nature)
- for a probability problem we can draw conclusions about characteristics of hypothetical data taken from the population based on known features of the population (deductive in nature)

**fundamental relationship between probability and inferential statistics**
```
         --------- probability ---------
        |                               |
    population                        sample    
        |                               |
         ---------- statistics ---------    

```
- the procedure involves two different jobs, thos are
    1.  to estimate a parameter of the population through sample
    2.  testing hypotheses or conjectures/claims about the parameter

## data collection and sampling procedures

- statistics deals not only with the organization and analysis of data once it has been collected but also with the development of techniques for collecting the data
- data not properly collected may be useless and misleading
- appropriate sampling scheme must be used
    - simple random sample:  any particular sample of a specified sample size has the same chance of being selected as any other sample of the same size
    - stratified random sample

## pictorial and tabular methods in descriptive statistics
visual representation of data is a powerful tool for understanding data, some examples are:

1. stem-and-leaf display

2. dotplots

3. histograms

4. boxplots

5. frequency tables

6. pie charts

7. bar graphs

8. scatterplots

### stem-and-leaf display

- a stemp and leaf plot, a combined tabular and graphic display, can be used to study the behavior of the mass statistical data
    - split each observation into 2 parts: stem and leaf
        - stem can be the digit preceding the decimal point
        - leaf can be the digit after the decimal point
    - make a table:  list the stem values as rows and ahh each leaf value with a specific stem value to that row

**example**  the following table show the life of 40 car batteries

```
2.2 4.1 3.5 4.5 3.2 3.7 3.0 2.6 
3.4 1.6 3.1 3.3 3.8 3.1 4.7 3.7 
2.5 4.3 3.4 3.6 2.9 3.3 3.9 3.1 
3.3 3.1 3.7 4.4 3.2 4.1 1.9 3.4 
4.7 3.8 3.2 2.6 3.9 3.0 4.2 3.5
```

<p style="color:blue;">stem (integer part) -and-leaf (decimal part) plot of battery life</p>

| stem | leaf          | frequency |
|:---- |:--------------|:----------|
| 1    | 69            | 2         |
| 2    | 25669         | 5         |
| 3    | 0011112223334445567778899 | 25 |
| 4    | 11234577      | 10        |

### dotplots

- there are two sample from separate populations.  the purpose is to determine if the use of the nitorgen has an influence on the growth of the roots
- in the **dot plot** 
    - ○ - the "nitrogen" data
    - x - the "no-nitrogen" data
- the data suggest on average the use of nitrogen increases the stem weight.  most of the no-nitrogen observations appear to be below the center of the data.  thus it indicates that nitrogen is effective.

| no-nitrogen | nitrogen |
|:------------|:---------|
0.32 | 0.26 | 
0.53 | 0.43 |  
0.28 | 0.47 | 
0.37 | 0.49 | 
0.47 | 0.52 | 
0.43 | 0.75 | 
0.36 | 0.79 | 
0.42 | 0.86 | 
0.38 | 0.62 |
0.43 | 0.46 |

<img width="700px" alt="step" src="https://user-images.githubusercontent.com/65584733/215172132-ce8622d2-4566-4f92-85fe-6ec919cc6642.png">

### histograms

- by rotating a stem-and-leaf plot counter clockwise through an angle of 90 degrees, the resulting columns of leaves form a picture that is similar to a histogram
- as the sample size becomes larger, the frequency histogram would approach a bell-shaped continuous probability distribution

<a href="https://commons.wikimedia.org/wiki/File:Histogram_of_arrivals_per_minute.svg#/media/File:Histogram_of_arrivals_per_minute.svg"><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/c/c3/Histogram_of_arrivals_per_minute.svg/1200px-Histogram_of_arrivals_per_minute.svg.png" alt="Histogram of arrivals per minute.svg" style="width:300px"></a>

## measures of location

- location measure in data set provide the analyst some quantitative measure of where the **data center** is in a sample mean.

### 1.  **sample mean**

- suppose that the observations in a smple are $x_{1}, x_{2}, x_{3}, \cdots, x_{n}$, the sample mean denoted $\bar{x}$

$$ \bar{x} = \frac{\sum_{i=1}^{n} x_{i}}{n} = \frac{x_{1} + x_{2} + \cdots + x_{n}}{n} $$

- sensitive to outliers (or extreme values)
- one obvious measure is the sample mean (mathematical average), which is simply a numerical average.
- the sample median is to reflect the central tendency of the sample and is uninfluenced by extreme values.

### 2.  **sample median** 

- middle value in the observations of ordered data set.  It divides a data set into two equal parts, denoted by $\tilde{x}$

- **if $n$ is even**

$$ \tilde{x} = \frac{x_{\frac{n+1}{2}} + x_{\frac{n+2}{2}}}{2} $$

- **if $n$ is odd**

$$ \tilde{x} = x_{\frac{n+1}{2}} $$

**example**

- a sample of n = 12 recording Beethovens Symphony #9, yielding the following durations (min) listed in increasing order is as follows

    62.3 62.8 63.6 65.2 65.7 66.4 67.4 68.4 68.8 70.8 75.7 79.0

    - the sample mean is 68.01

    - the sample median is the average of the $n/2 = 6\text{th}$ and $n/2 + 1 = 7\text{th}$ observations
    - note:  if the largest observation 79.0 was excluded from the sample, the resulting sample median for the n = 11 remaining observations would have been the single middle value 66.4 (the [n +1] = 2 6th ordered value, i.e. the 6th value in from either end of the ordered list
    - the sample mean is $\bar{x} = 68.01$ and the sample median is $\tilde{x} = 67.4$

### 3.  **quartiles** 
- divide the data set (sample or population) into four equal parts
- observations above the third quartile are Q3 constituting the upper quarter of the data set
- the second quartile Q2 is the median
- the first quartile Q1 separates the lower quarter from the upper three-quarters

**example**  beethovens symphony #9

- data: $Q_{1} = 64.80$, $Q_{2} = 66.90$, $Q_{3} = 69.30$
- a data set (sample or population) can be even more finely divided using **percentiles**; the 99th percentile separates the highest 1% from the bottom 99%, and so on.
- the mean is quite sensitive to a single outlier, whereas the median is not.  the median is a more robust measure of central tendency than the mean.

### 4.  **trimmed mean**

- a trimmed mean is comprised betweeen $\bar{x}$ and $\tilde{x}$, and is a more robust measure of central tendency than the mean.  

**example**

- the 10% trimmed mean is found by eliminating the largest 10% and smallest 10% and computing the average of the remaining values
- so, for the with nitrogran group the 10% trimmed mean is 

**observations of nitrogen influences**

| no-nitrogen | nitrogen |
|:------------|:---------|
| 0.32 | 0.26 | 
| 0.53 | 0.43 |  
| 0.28 | 0.47 | 
| 0.37 | 0.49 | 
| 0.47 | 0.52 | 
| 0.43 | 0.75 | 
| 0.36 | 0.79 | 
| 0.42 | 0.86 | 
| 0.38 | 0.62 |
| 0.43 | 0.46 |

$$ \bar{x_{tr(10)}} = \frac{0.43 + 0.47 + 0.49 + 0.52 + 0.75 + 0.79 + 0.62 + 0.46}{8} = 0.56 $$

## measures of variability

- location measures no not provide a proper summary of the **nature of the data set**.
- we can not make meaningful conclusions without considering sample variability
- some measures of variability 
    - range (max - min)
    - interquartile range (Q3 - Q2)
    - variance or standard deviation
- different samples or populations may have identical measures of center yet differ from one another in important ways.

**example** 

<img width="400px" alt="Screenshot 2023-01-27 at 1 17 39 PM" src="https://user-images.githubusercontent.com/65584733/215177381-c007cc97-2661-435b-bce1-02aea2cd3516.png">

<br>

### 1.  **sample range**

- simplest measure of sample variability is the sample range $X_{max} - X_{min}$
- **interquartile range (IQR)** between the 75th percentile **(upper quartile)** and the 25th percentile **(lower quartile)**
- the range can be very useful in statistical quality control
- the question "how far is each x from the mean?", the one that is used most often is the sample standard deviation

### 2.  **sample variance**

the sample variance of $X_{1}, X_{2}, \cdots, X_{n}$ is denoted by $\sigma^{2}$

$$
\sigma^{2} = s^{2} = \frac{1}{n - 1} \sum_{i=1}^{n} (x_{i} - \bar{x})^{2}
$$

### 3.  **sample standard deviation**

the sample standard deviation denoted by $s$ is the positive square root of the sample variance

$$
s = \sqrt{s^{2}}
$$

- both $s^{2}$ and $s$ are both nonnegative.  the unit for $s$ is the same as the unit for each of the $x_{i}s$

### 4.  **five-number summaries and boxplots**

- with $x_{1}, x_{2}, \cdots, x_{n}$, the five-number summary is given by the minimum, first quartile Q1, median, third quartile Q3, maximum.
- a boxplot (box-and-whisker plot) is a way of graphically depicting groups of numerical data through their five-number summaries
- a graphical tool to get an idea about the center, variability, and degree of asymmetry of sample
- box-and-whisker plot enclosed the interquartile range of the data in a box that has median displayed within.
- boxplot provides the viewer information about outliers which represent rare events

<img src="https://www.isixsigma.com/wp-content/uploads/2019/07/Anatomy-of-a-Box-Plot.gif">

- nicotine content was measured in a random sample of 40 cigarettes.  the data is displayed in the table
- mild outliers:  0.72, 0.85, 2.55

**table nicotine data**

<img width="457" align="right" alt="Screenshot 2023-01-27 at 1 40 04 PM" src="https://user-images.githubusercontent.com/65584733/215182735-b3474169-f997-4af5-9a49-4c5e0173f73a.png">

```
1.09 1.92 2.31 1.79 2.28 1.74 1.47 1.97
0.85 1.24 1.58 2.03 1.70 2.17 2.55 2.11 
1.86 1.90 1.68 1.51 1.64 0.72 1.69 1.85 
1.82 1.79 2.46 1.88 2.08 1.67 1.37 1.93 
1.40 1.64 2.09 1.75 1.63 2.37 1.75 1.69
```



## discrete and continuous data

## general types of statistical studies


# ch 02 probability

**contents**

1.  [sample space](#sample-space)
2.  [events](#events)
3.  [counting sample points](#counting-sample-points)
4.  [additive rules](#additive-rules)
5.  [conditional probability](#conditional-probability)
6.  [multiplicative rules](#multiplicative-rules)
7.  [bayes' rule](#bayes-rule)
8.  [exercises](#chapter-2-probability)

## sample space

**the sample space of an experiment**

- an experiment is any activity or process that generates (or observes) a set of data and the data are subject to uncertainty

- experiments that may be of interest include
    - tossing a coin once or several times
    - selecting a card from a deck of cards
    - weighing a loaf of bread
    - ascertaining the commuting time from home to work on a particular morning
    - obtaining blood types from a group of individuals

- tossing a coin example

$$
    S = \{H, T\} \\
    P(H) = \frac{1}{2} \newline   
    P(T) = \frac{1}{2} \newline
$$

- the member of the sample space or the elements

**definition 2.1** the set of possible outcomes of a statistical experiment is called the **sample space**, represented by S.

- each outcome in the sample space is called
    - an element of the sample space
    - a member of the sample space
    - a sample point

- if the sample space has a finite number of elements, we may list the members
- if the sample space has a large or infinite number of elements, we describe it by a **statement** or **rule**.

**example**
- topssing a coin $S = \{H, T\}$
- tossing a die
- $S = \{1, 2, 3, 4, 5, 6\}$
- $S = \{{odd}, {even}\}$
- $S = \{ x | x \in \mathbb{R}, 2 ≤ x ≤ 4\}$
- $S = \{ x | x \text{is a city with population of 1 million or more} \}$

**tree diagrams** can be used to list the elements of the sample space systematically

**example**  

- flip a coin first, if head occurs, flip it again; otherwise, toss a die
- $S = \{HH, HT, T_{1}, T_{2}, T_{3}, T_{4}, T_{5}, T_{6}\}$

## events

**definition 2.2** an event is a subset of a sample space
- **null set** denoted by $\emptyset$ is an event that contains no elements

**definition 2.3**  the **complement** of an event $A$ with respect to $S$ is the subset of all elements of $S$ that are not in $A$.  We denote the complement of $A$ as the symbol $A'$

- **example**  let $R$ be the event that a red card is selected from an ordinary deck of 52 playing cards.
- $S$ be the entire deck
- $R'$ is the event that the card selected from the deck is not red but a black card.

**definition 2.4**  the **intersection** of two events $A$ and $B$, denoted by the symbol $A \cap B$, is the event containng all elements that are common to $A$ and $B$.

- **example** let $P$ be the event that a person selected at random while dining at a popular cafeteria is a taxpayer.  
    - $Q$ is the event that the person is over 65 years of age
    - the event $P \cap Q$ is the set of all taxpayers in the cafeteria who are over 65 years of age.

**definition 2.5**  the two events $A$ and $B$ are **mutually exclusive** or **disjoint** if $A \cap B = \emptyset$, i.e. if $A$ and $B$ have no elements in common.  two events can not occur simultaneously.

- **example** 
    - let $A$ be the event that the program belongs to the NBC network.
    - let $B$ be the event that the program belongs to the CBS network.
    - $A$ and $B$ are mutually exclusive.

**definition 2.6**  the **union** of the two events $A$ and $B$, denoted by the symbol $A \cup B$, is the event containing all the elements that belong to $A$ or $B$ or both.

- **example**
    - if $M = \{x | 3 < x < 9\}$ and $N = \{y | 5 < y < 12\}$
    - then $M \cup N = \{x | 3 < x < 12\}$

**venn diagram**
- let the sample space be a rectangle and represent events by circles.
- the relationship between events and the corresponding sample space can be illustrated graphically by Venn Diagram.

<img align="center" style="width: 300px;" src="https://user-images.githubusercontent.com/65584733/215618926-9c41e882-b93f-42bf-b21f-2ba8f10ec94b.jpg">

**properties**
- $A \cup B$ is 7, 4, 2, 1, 6, 3
- $A \cap C$ is 2, 1
- $B' \cap A$ is 7, 4
- $A \cap B \cap C$ is 1
- $(A \cup B) \cap C'$ is 2, 7, 6

**example**  flip a coin first, if a head occurs, flip it again; otherwise toss a die.

$S = \{HH, HT, T_{1}, T_{2}, T_{3}, T_{4}, T_{5}, T_{6}\}$

<img align="center" style="width: 300px;" src="https://user-images.githubusercontent.com/65584733/215615608-476198ef-d341-4b86-a286-669eba51efd2.jpg">

<br>

**example**  three items are selected at random from a process

$S = \{DDD, DDN, DND, DNN, NDD, NDN, NND, NNN\}$

<img align="center" style="width: 300px;" src="https://user-images.githubusercontent.com/65584733/215616113-251e0905-3b2c-4cea-929c-996c0dcde2f4.jpg">

**event operations**
- $A \cap \emptyset = \emptyset$
- $A \cup \emptyset = A$
- $A \cap A' = \emptyset$
- $A \cup A' = S$
- $S' = \emptyset$
- $\emptyset' = S$
- $(A \cap B)' = A' \cup B'$
- $(A \cup B)' = A' \cap B'$

## counting sample points

- **combinatorics** - counting rules in set theory.  this provides the idea of the principles of enumeration, counting samplw ponts in the **sample space**
- when an experiment is performed, the statisticin wants to evaluate the change with the occurence of certain events.
- in many cases we can evaluate the probability by counting the number of points in the sample space.

**theorem 2.1 multiplicative rule**

if an operation can be performed in $n_{1}$ ways, and if for each of these a second operation can be performed in $n_{2}$ ways, then the two operations can be performed together in $n_{1}$ $n_{2}$ ways.

- the multiplication rule is the fundamental principle of counting sample points.

**theorem 2.2 generalized multiplicative rule**

if an operation can be performed in $n_{1}$ ways, and if for each of these a second operation can be performed in $n_{2}$ ways, and for each of the first two a third operation can be performed in $n_{3}$ ways, and so forth, then the sequence of $k$ operation can be performed in $n_{1}$ $n_{2}$ $\dots$ $n_{k}$

**example 2.16** how many even four-digit numbers can be formed form the digits 0, 1, 2, 5, 6, and 9 if each digit can be used only once?

- we consider the unit position by two parts, 0, or not 0
    - if the units opsition is $0(n_{1} = 1)$
    - $n_{2} = 5$ choices for the thousands position
    - $n_{3} = 4$ choices for the hundreds position

**def 2.7 permutation**

a permutation is an arrangemnet of all or part of a set of objects

- an **ordered** arrangement of distinct objects.  For example, consider the number of ways of filling r boxes with n objects.

**theorem 2.3 permutation**

the number of permutations of $n$ objects is $n!$

**theorem 2.4 permutation**

the number of permutation (ways to arrange) of $n$ distinct objects taken $r$ at a time is

$$
P(n, r) = \frac{n!}{(n-r)!} \\
$$

**example**  in one year, three awards will be given for a class of 25 graduate student.
- if each student can receive at most one award, how many possible selection are there?
- since the awards are *distingioshable*, it is a permutation problem with $n = 25$ and $r = 3$.
- the number of sample points is $P(25, 3) = \frac{25!}{(25-3)!} = 25 \times 24 \times 23 = 17, 400$

**theorem 2.8**  the number of combinations (ways of choosing, **regardless of order** of $n$ distinct objects taken $r$ at a time is...

"n choose r"
$\binom{n}{r} = \frac{n!}{r!(n-r)!}$

- we might want to select $r$ objects from $n$ without regard to order
- these selections are called **combinations**
- combinations are used when we are sampling without replacement and order does not matter
- a combination is a partition with two cells,
    - the one containing the $r$ objects selected
    - the other containing the remaining $n-r$ objects
- the number of such combinations is

**summary**

**permutation** - order matters the number of permutations of $n$ objects is
$$ 
n! = n \times (n-1) \times (n-2) \times \dots \times 2 \times 1
$$

**permutation** - order matters the number of permutations of $n$ distinct objects taken $r$ at a time

$$
P(n, r) = \frac{n!}{(n-r)!}
$$

**combination** - order does not matter

$$
C(n, r) = \binom{n}{r} = \frac{n!}{r!(n-r)!}
$$

### probability of event

- the likelihood of the occurrences of an event resulting of a statistical experiment is evaluated by means of a set of real number called weights or probabilities range from 0 to 1.

- the probability is a numerical measure of the likelihood of occurrence of an event, denoted by $P(A)$

- to every point in the sample space we assign a probability such that the sum of all probabilities is 1.

- for points outside the sample space i.e. for events that cannot possibly occur, we assign a probability of 0.

**definition 2.8**

the probability of an event A is the sum of the weights of all sample points in A

$$
0 \leq P(A) \leq 1 \\
P(\varnothing) = 0 \\
P(S) = 1 \\
$$

if $A_{1}, A_{2}, \dots, A_{n}$ are disjoint events, then the probability of the union of these events is the sum of the probabilities of the individual events

$$
P(A_{1} \cup A_{2} \cup \dots \cup A_{n}) = P(A_{1}) + P(A_{2}) + \dots + P(A_{n}) \\
$$

- in fact, p is a probability set function of the outcomes of the random experiment, which tells us how the probability is distributed over various subsets A of a sample space S.

**example** a coin is tossed twice 
    - what is the probability that at least one head occur?
    - we assign a probability $w$ to each sample point
    - then 4w = 1

$$
S = \{HH, HT, TH, TT\}, A = \{HH, HT, TH\} \\
P(A) = \frac{1}{4} + \frac{1}{4} + \frac{1}{4} = \frac{3}{4} \\
$$

**theorem** 2.9

if an experiment can result in any one of $N$ different equally likely outcomes, and if exactly $n$ of these outcomes correspond to event $A$, then the probability of event $A$ is,

$$
P(A) = \frac{n}{N} \\
$$

**example**  in a poker hand consisting of 5 cards, find the probability of holding 2 aces and 3 jacks is,


$$
\binom{52}{5} = \frac{52!}{5!(52-5)!} = 2, 598, 960 \\
$$

$$
P(C) = \frac{C(4, 2) \times C(4, 3)}{C(52, 5)} = \frac{\frac{4!}{2!2!} \times \frac{4!}{3!1!}}{\frac{52!}{5!47!}} = \frac{24}{2598960} = 0.000009234463016\\
$$

- if the outcomes of an experiment are not equally likely to occur, the probabilities must be assigned based on prior knowledge or experimental evidence
- the use of intuition, personal beliefs, and other indirect information in arriving at probabilities is reffered to as the subjective definition of probability
- according to the relative frequency definition of probability, the true probabilities would be the fractions of events that occur in the long run

## additive rules

**theorem 2.10** if A and B are two events, then the probability of the union of A and B is

$$
P(A \cup B) = P(A) + P(B) - P(A \cap B) \\
$$

**corollary 1**  if A and B are mutually exclusive, then,

$$
P(A \cup B) = P(A) + P(B) \\
$$

**corollary 2** if $A_{1}, A_{2}, \dots, A_{n}$ are mutually exclusive events, then

$$
P(A_{1} \cup A_{2} \cup \dots \cup A_{n}) = P(A_{1}) + P(A_{2}) + \dots + P(A_{n}) \\
$$

- a collection of events $\{A_{1}, A_{2}, \dots, A_{n}\}$ of a sample space $S$ is called a partition of $S$ if $A_{1}, A_{2}, \cdots, A_{n}$ are mutually exclusive and $A_{1} \cup A_{2} \cup \cdots \cup A_{n} = S$

## conditional probability

**conditional probability** $P(A|B)$

- sometimes the occurrence of an event is influenced or related with some other event
- hence we must take this restriction or the availability of certain limited information into consideration about the outcome of the experiment.
- "the probability of an event $B$ occurs given that $A$ occurs"

## multiplicative rules

- multiplying the formula of definition 2.9 (shown below) by $P(A)$, we obtain the **multiplicative rule**, which enables us to calculate the probability that two events will both occur.

**definition 2.9**

$$
P(B | A) = \frac{P(A \cap B)}{P(A)} \\
\text{if } P(A) > 0 \\
$$

## bayes' rule

**theorem 2.17**  if the events $B_{1}, B_{2}, \dots, B_{n}$ constitute a partition of the sample space $S$ such that $P(B_{i}) ≠ 0$ for $i = 1, 2, \dots, k$, then

$$
P(B_{r} | A) = \frac{P(B_{r} \cap A)}{\sum_{i = 1}^{k} P(B_{i} \cap A)} = \frac{P(B_{r} \cap A)}{\sum_{i = 1}^{k} P(B_{i} | A) P(B_{i})}
$$

- it can be proved by the definition of conditional probability, with using the theorem 2.16 in the denominator

$$
P(B_{r} | A) = P(B_{r} \cap A) / P(A) 
$$

- useful in problems where $P(B_{i} | A)$ are not known but $P(A | B_{i})$ and $P(B_{i})$ are known,

- $P(B_{i})$ are **priors**
- $P(A | B_{i})$ are **likelihoods**
- $P(B_{i} | A)$ are **posteriors**

# chapter 2 probability

morgan bergen

math 526 applied mathematical statistics 1

jan 31 2023

**exercises**

[2.14](#214), [2.34](#234), [2.36](#236), [2.50](#250), [2.56](#256), [2.60](#260), [2.78](#278), [2.82](#282), [2.95](#295), [2.100](#2100)

## 2.14

**if $S = \{0, 1, 2, 3, 4, 5, 6, 7, 8, 9\}$ and $A = \{0, 2, 4, 6, 8\}$, $B = \{1, 3, 5, 7, 9\}$, $C = \{2, 3, 4, 5\}$, and $D = \{1, 6, 7\}$, list the elements of the sets corresponding to the following events:**
    
**a.  $A \cup B$** $= \{0, 1, 2, 3, 4, 5, 6, 7, 8, 9\}$

**b.  $A \cap B$** $= \{0, 2, 4, 6, 8\}$

**c.  $C'$** $= \{0, 1, 6, 7, 8, 9\}$

**d.  $(C' \cap D) \cup B$** $= \{1, 6, 7, 3, 5, 9\}$

**e.  $(S \cap C)'$** $= \{0, 1, 6, 7, 8, 9\}$

**f.  $A \cap C \cap D'$** $= \{2, 4\}$

## 2.34

**a.  how many distinct permutations can be made from the letters of the word _COLUMNS_?**

$C = n_{1}, O = n_{2}, L = n_{3}, M = n_{4}, U = n_{5}, S = n_{6}$
where there are total $n = 7$ elements and no letter can appear no more than just once therefore according to the fundamental counting principle there are $n! = 7! = 5040$ permutations

**b.  how many of these permutations start with the letter _M_?**

the required number of permutations where $M = n_{4}$ is fixed at the first index position leaves there to be $n - 1 = 6$ elements to be permuted therefore there are $n! = 6! = 720$ permutations.
## 2.36

**a.  how many three-digit numbers can be formed from the digits 0, 1, 2, 3, 4, 5, 6 if each digit can be used only once?**

<img src="https://user-images.githubusercontent.com/65584733/217289039-4407d8a6-84ad-4b7a-91ff-cd0aeb77de1c.png" width="200" height="200">

there are 7 unchosen digits to choose from in total.  
- for index position 0 there are 6 digits to choose from other than 0 (say we choose 1)
- for index position 1 there are 6 digits to choose from other than 1 (say we choose 0)
- for index position 2 there are 5 digits to choose from other than 0 and 1 (say we choose 2)
therefore there are $(6)*(6)*(5) = 180$ three-digit numbers that can be formed from the digits 0, 1, 2, 3, 4, 5, 6 if each digit can be used only once.

**b.  how many of these are odd numbers?**

<img src="https://user-images.githubusercontent.com/65584733/217299141-90850f84-b3e7-48f8-975f-f6e3ae82be53.png" width="200" height="200">

there are 7 unchosen digits to choose from in total
- for index position 2 there are 3 digits to choose from since the only odd digis are 1, 3, 5 (say we choose 5)
- for index position 0 there are 5 digits to choose from since 0 can't be the first digit and 5 is already chosen (say we choose 1)
- for index position 1 there are 5 digits to choose from since 1 and 5 are already chosen (say we choose 0)
therefore there are $(5)*(5)*(3) = 75$ odd numbers that can be formed from the digits 0, 1, 2, 3, 4, 5, 6 if each digit can be used only once.

**c.  how many are greater than 330?**

case 1:  greater than 330 and less than 400 (precisely 340 ≤ x ≤ 365)
- index 0 has 1 choice since we are only considering 3 (say we choose 3)
- index 1 has 3 choices since we are only considering 4, 5, 6 (say we choose 4)
- index 2 has 5 choices since we exclude 3, 4 (say we choose 0)
so, there are $(1)*(3)*(5) = 15$ for case 1

case 2:  greater than 400 (precisely 401 ≤ x ≤ 654)
- index 0 has 3 choices since we are only considering greater than 3, so 4, 5, 6 (say we choose 4)
- index 1 has 6 choices since we are excluding 4 (say we choose 0)
- index 2 has 5 choices since we exclude 4, 0 (say we choose 1)
so, there are $(3)(6)(5) = 90$ for case 2

therefore, case 1 + case 2 = $(1)*(3)*(5) + (3)(6)(5) = 105$ numbers greater than 330


<img src="https://user-images.githubusercontent.com/65584733/217298997-0b3b6e1f-5fc6-4ebb-84fc-ec975d0f36c4.png" height="300">


## 2.37

**in how many ways can 4 boys and 5 girls sit in a row if the boys and girls must alternate?**

according to the fundamental counting principle if an operation can be performed in $n_{1}$ ways, and if for each of these a second operation can be performed in $n_{2}$ ways, then these two operations can be performed together in $n_{1} * n_{2}$ ways.

$S = \{b, b, b, b, g, g, g, g, g\}$
- the first operation which consists of the number of permutations of 5 girls is $n_{1} = 5! = 120$ different ways
- the second operation which consists of the number of permutations of 4 boys is $n_{2} = 4! = 24$ different ways
- therefore $n_{1} * n_{2} = 120 * 24 = 2880$ ways in which 4 boys and 5 girls can sit in a row with the given condition that boys and girl must alternate.

## 2.50

**assuming that all elements of $S$ in exercise 2.8 on page 42 are equally likely to occur, find**

**a.  the probability of event $A$**

$P(A) = 10(1/36) = 10/36 = 5/18$

**b.  the probability of event $C$**

$P(C) = 12(1/36) = 12/36 = 1/3$

**c.  the probability of event $A \cap C$**

$P(A \cap C) = 7(1/36) = 7/36 = 7/108$

<img src="https://user-images.githubusercontent.com/65584733/217575279-388eb3d0-bc96-41f2-8d64-8c77b3c36c07.png" height="850">

## 2.56

**an automobile manufacturer is concerned about a possible recall of its best-selling four-door sedan.  if there were a recall, there is a probability of 0.25 of a defect in the brake system, 0.18 of a defect in the transmission, 0.17 of a defect in the fuel system, and 0.40 of a defect in some other area.**

**a.  what is the probability that the defect is the brakes or the fueling system if the probability of defects in both systems simultaneously is 0.15?**

"both systems simultaneously" 
- means that the probability of the defect being in both is $0.15$
- $P(B \cap F) = 0.15$

"what is the probability that the defect is the brakes or fueling system" 
- since we were given $P(B \cap F) = 0.15$
- $P(B \cup F) = P(B) + P(F) - P(B \cap F)$
- $P(B \cup F) = 0.25 + 0.17 - 0.15 = 0.27$
- $P(B \cup F) = 0.27$
- therefore the probability that the defect is the brakes or fueling system is $0.27$

**b.  what is the probability that there are no defects in either the brakes or the fueling system?**

"no defects in either the brakes or fueling system"
- means that the probability of the defect is not in either which is complementary to $P(B \cup F)$
- $P(B \cup F)' = 1 - P(B \cup F)$
- $P(B \cup F)' = 1 - 0.27 = 0.73$

<img src="https://user-images.githubusercontent.com/65584733/217625296-89b01780-141a-4e9d-be41-13fcf961520f.png" width="850">


## 2.60

**if 3 books are picked at random from a shelf containing 5 novels, 3 books of poems, and a dictionary, what is the probability that**

the number of combinations (ways of choosing, regardless of order and without replacement) of $N = 9$ distinct objects taken $R = 3$ at a time is found in theorem 2.8 of combinatorics

$S = \{n_{1}, n_{2}, n_{3}, n_{4}, n_{5}, p_{1}, p_{2}, p_{3}, d\}$

$\binom{N}{R} = \frac{N!}{R!(N-R)!}$ 

$\binom{9}{3} = \frac{9!}{3!(9-3)!} = \frac{9!}{(3!)(6!)} = \frac{9(8)(7)}{3(2)(1)} = \frac{504}{6} = 84$

- where $N = 9$ is the total number of objects
- and $R = 3$ is the number of objects to be chosen

**a.  the dictionary is selected?**

- number of ways to select 1 dictionary and 2 other books is,
- $\binom{1}{1}\binom{8}{2} = \frac{1!}{1!(1-1)!}\frac{8!}{2!(8-2)!} = \frac{1}{1}\frac{8(7)}{2(1)} = 28$
- therefore, the probability of selecting the dictionary is $28/84 = 7/21 = 1/3$

**b.  2 novels and 1 book of poems are selected?**

- number of ways to select 2 novels and 1 poem is,
- $(\binom{5}{2})(\binom{3}{1}) = (\frac{5!}{2!(5-2)!})(\frac{3!}{1!(3-1)!}) = (\frac{(5)(4)}{(2)(1)})(\frac{3}{1}) = 30$
- therefore the probability of selecting 2 novels and 1 poem is $30/84 = 5/14$

<img src="https://user-images.githubusercontent.com/65584733/217662549-c2f67eb2-2fe4-4627-9aeb-e299ba8d59d9.png" width="850">


## 2.78

**a manufacturer of a flu vaccine is concerned about the quality of its flu serum.  batches of serum are processed by three different departments having rejection rates of 0.10, 0.08, 0.12 respectively.  the inspections by the three departments are sequential and independent**

- let $P(R_{1}) = 0.10$ be the rejection rate of the first department
- let $P(R_{2}) = 0.08$ be the rejection rate of the second department
- let $P(R_{3}) = 0.12$ be the rejection rate of the third department
- given that the events are independent and sequential means that the probability of the event is the product of the probabilities of the individual events
- $P(R_{1} \cap R_{2} \cap R_{3}) = P(R_{1}) * P(R_{2}) * P(R_{3}) = 0.10 * 0.08 * 0.12 = 0.0096$

**a.  what is the probability that the batch of serum survives the first departmental inspection but is rejected by the second department?**

- let $P(A_{1}) = 1 - P(R_{1}) = 1 - 0.10 = 0.90$ be the probability that the batch of serum survives the first departmental inspection
- let $P(A_{2}) = 1 - P(R_{2}) = 1 - 0.08 = 0.92$ be the probability that the batch of serum survives the second departmental inspection
- let $P(A_{3}) = 1 - P(R_{3}) = 1 - 0.12 = 0.88$ be the probability that the batch of serum survives the third departmental inspection

therefore, the probability that the first departmental inspection is passed and the second departmental inspection is rejected is, $P(A_{1} \cap R_{2}) = (0.9)(0.08) = 0.072$

![a](https://user-images.githubusercontent.com/65584733/217669608-e60e037d-ad74-4128-b3b9-43cdc6234d63.png)

**b.  what is the probability that a batch of serum is reject by the third department?**

- since the events are sequential in nature, a batch that was reject by the third department implies that the first and second batch are rejected, therefore $P(A_{1} \cap A_{2} \cap R_{3}) = (0.9)(0.92)(0.12) = 0.09936$

![a](https://user-images.githubusercontent.com/65584733/217670715-3a2d6e71-f733-430c-9bf2-4e3b5521f91d.png)

## 2.82

**for married couples living, in a certain suburb, the probability that the husband will vote on a bond referendum is 0.21, the probability that the wife will vote on the referendum is 0.28, and the probability that both the husband and the wife will vote is 0.15.  what is the probability that**

- the following is given in the question,
- $P(H) = 0.21$ is the probability that the husband will vote
- $P(W) = 0.28$ is the probability that the wife will vote
- $P(W') = 1 - P(W) = 1 - 0.28 = 0.72$ is the probability that the wife will not vote
- $P(H') = 1 - P(H) = 1 - 0.21 = 0.79$ is the probability that the husband will not vote
- $P(H \cap W) = 0.15$ is the probability that both the husband and the wife will vote

**a.  at least one member of a married couple will vote?**

- $P(H \cup W) = P(H) + P(W) - P(H \cap W) = 0.21 + 0.28 - 0.15 = 0.34$

**b.  a wife will vote, given that her husband will vote?**

- $P(W|H) = \frac{P(H \cap W)}{P(H)} = \frac{0.15}{0.21} = 0.714$

**c.  a husband will vote, given that his wife will not vote?**

- $P(H|W') = \frac{P(H \cap W')}{P(W')} = \frac{P(H/(H \cap W))}{P(W')} = \frac{P(H) - P(H \cap W)}{P(W')} = \frac{0.21 - 0.15}{0.72} = 0.083$

## 2.95

**in a certain region of the country it is known from past experience that the probability of selecting an adult over 40 years of age with cancer is 0.05.  if the probability of a doctor correctly diagnosing a person with cancer as having the disease is 0.78 and the probability of incorrectly diagnosing a person without cancer as having the disease is 0.06, what is the probability that an adult over 40 years of age is diagnosed as having cancer?**

- $P(C) = 0.05$

- $P(C') = 1 - P(C) = 1 - 0.05 = 0.95$

- $P(D | C) = 0.78$

- $P(D | C') = 0.06$

$$
P(D) = P(D | C)(P(C)) + P(D|C')(P(C')) = (0.78)(0.05) + (0.06)(0.95) = 0.096
$$

## 2.100

**a regional telephone company operates three identical relay stations at different locations.  during a one-year period, the number of malfunctions reported by each station and the causes are shown below**

| station | A | B | C |
|:--------|:-:|:-:|:-:|
| problems with electricity supplied | 2 | 1 | 1 |
| computer malfunction | 4 | 3 | 2 |
| malfunctioning electrical equipment | 5 | 4 | 2 |
| caused by other human errors | 7 | 7 | 5 |

**suppose that a malfunction was reported and it was found to be caused by other human errors.  what is the probability that it came from station C?**

- $P(E)$ be the probability that a malfunction by other human errors

$$P(C | E) = \frac{P(E|C)(P(C))}{P(E|A)P(A) + P(E|B)P(B) + P(E|C)P(C)} = \frac{(5/10)(10/43)}{(7/18)(18/43)+(7/15)(15/43)+(5/10)(10/43)}= \frac{0.1163}{0.4419} = 0.2631876711$$


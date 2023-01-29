# ch 02 probability

**contents**

1.  [sample space](#sample-space)
2.  [events](#events)
3.  [counting sample points](#counting-sample-points)
4.  [additive rules](#additive-rules)
5.  [conditional probability](#conditional-probability)
6.  [multiplicative rules](#multiplicative-rules)
7.  [bayes' rule](#bayes-rule)

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
    S = \{H, T\} \newline
    P(H) = \frac{1}{2} \newline 
    P(T) = \frac{1}{2} \newline
$$

- the member of the sample space or the elements

**definition 2.1** the set of possible outcomes of a statistical experiment is called the **sample space**, represented by S.

- each outcome in the sample space is called
    - an element of the sample space
    - a member of the sample space
    - a sample point

- if the sample space has a large or infinite number of elements, we describe it by a state or rule

**example 2.1**

- topssing a coin $S = \{H, T\}$
- tossing a die
    - $S = \{1, 2, 3, 4, 5, 6\}$
    - $S = \{{odd}, {even}\}$
- $S = \{ x | x \in \mathbb{R}, 2 ≤ x ≤ 4\}$
- $S = \{ x | x $ is a city with population of 1 million or more \}$

- a tree diagram can be used to list the elements of the sample space systematically

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
$$
\binom{n}{r} = \frac{n!}{r!(n-r)!} \\
$$

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
P(n, r) = \frac{n!}{(n-r)!} \\
$$

**combination** - order does not matter

$$
C(n, r) = \binom{n}{r} = \frac{n!}{r!(n-r)!} \\
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
P(\empty) = 0 \\
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

- a collection of events $\{A_{1}, A_{2}, \dots, A_{n}\}$ of a sample space $S$ is called a 


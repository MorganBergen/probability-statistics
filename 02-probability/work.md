# chapter 2 probability

morgan bergen

math 526 applied mathematical statistics 1

jan 31 2023

**exercises**

[2.14](#214)

[2.34](#234)

[2.36](#236)

[2.50](#250)

[2.56](#256)

[2.60](#260)

[2.78](#278)

[2.82](#282)

[2.95](#295)

[2.100](#2100)

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

## 2.82

**for married couples living, in a certain suburb, the probability that the husband will vote on a bond referendum is 0.21, the probability that the wife will vote on the referendum is 0.28, and the probability that both the husband and the wife will vote is 0.15.  what is the probability that**

**a.  at least one member of a married couple will vote?**

**b.  a wife will vote, given that her husband will vote?**

**c.  a husband will vote, given that his wife will not vote?**

## 2.95

**in a certain region of the country it is known from past experience that the probability of selecting an adult over 40 years of age with cancer is 0.05.  if the probability of a doctor correctly diagnosing a person with cancer as having the disease is 0.78 and the probability of incorrectly diagnosing a person without cancer as having the disease is 0.06, what is the probability that an adult over 40 years of age is diagnosed as having cancer?**

## 2.100

**a regional telephone company operates three identical relay stations at different locations.  during a one-year period, the number of malfunctions reported by each station and the causes are shown below**

| station | A | B | C |
|:--------|:-:|:-:|:-:|
| problems with electricity supplied | 2 | 1 | 1 |
| computer malfunction | 4 | 3 | 2 |
| malfunctioning electrical equipment | 5 | 4 | 2 |
| caused by other human errors | 7 | 7 | 5 |

**suppose that a malfunction was reported and it was found to be caused by other human errors.  what is the probability that it came from station C?**

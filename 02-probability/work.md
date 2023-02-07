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

there are 7 unchosen digits to choose from in total.  
- for index position 0 there are 6 digits to choose from other than 0 (say we choose 1)
- for index position 1 there are 6 digits to choose from other than 1 (say we choose 0)
- for index position 2 there are 5 digits to choose from other than 0 and 1 (say we choose 2)

**b.  how many of these are odd numbers?**

**c.  how many are greater than 330?**

## 2.37

**in how many ways can 4 boys and 5 girls sit in a row if the boys and girls must alternate?**

## 2.50

**assuming that all elements of $S$ in exercise 2.8 on page 42 are equally likely to occur, find**

**a.  the probability of event $A$**

**b.  the probability of event $C$**

**c.  the probability of event $A \cap C$**

## 2.56

**an automobile manufacturer is concerned about a possible recall of its best-selling four-door sedan.  if there were a recall, there is a probability of 0.25 of a defect in the brake system, 0.18 of a defect in the transmission, 0.17 of a defect in the fuel system, and 0.40 of a defect in some other area.**

**a.  what is the probability that the defect is the brakes or the fueling system if the probability of defects in both systems simultaneously is 0.15?**

**b.  what is the probability that there are no defects in either the brakes or the fueling system?**

## 2.60

**if 3 books are picked at random from a shelf containing 5 novels, 3 books of poems, and a dictionary, what is the probability that**

**a.  the dictionary is selected?**

**b.  2 novels and 1 book of poems are selected?**

## 2.78

**a manufacturer of a flu vaccine is concerned about the quality of its flu serum.  batches of serum are processed by three different departments having rejection rates of 0.10, 0.08, 0.12 respectively.  the inspections by the three departments are sequential and independent**

**a.  what is the probability that the batch of serum survives the first departmental inspection but is rejected by the second department?**

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

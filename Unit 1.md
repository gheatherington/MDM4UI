## Choosing
$$
\begin{gather*}
\text{If events are independent of each other:} \\
\text{Possible Paths: } m \cdot n \\
m, n \text{ are } \# \text{ of possibilities} \\ \\ 
\text{When sitting people around a round table:} \\
(n-1)!
\end{gather*}
$$
# Factorial Notation
$$
\begin{gather*}
n! = n \cdot (n-1) \cdot (n-2) \cdots 3 \cdot 2 \cdot 1 \\
\text{Example: }7! = 7 \cdot 6 \cdot 5 \cdot 4 \cdot 3 \cdot 2 \cdot 1 \\ \\
\text{Note: } 0! = 1
\end{gather*}
$$
# Arrangements with Repeated Elements
$$
\begin{gather*}
n \text{ objects, where:} 
a, b, c \text{ are alike} \\
\frac{n!}{a!b!c!}
\end{gather*}
$$

# Permutations
- An arrangement of items that need to appear in a ***DEFINITE ORDER - UNIQUE POSITIONS***
- In general, the number of arrangements of $n$ objects in $k$ positions is given by:
$$
{}_nP_k=\frac{n!}{(n-k)!}
$$

# Choose Function
* A collection of chosen items for which order is *NOT* (***NO SPECIFIC POSITION***)important ($abc=bac$)
* The number of ways to choose $r$ objects from a group of $n$ objects
$$
\begin{gather*}
{n \choose r} = \frac{n!}{(n-r)!\cdot r!}\\ \\
{n \choose r} = {n \choose (n-r)} \\
\text{Example: }
{30 \choose 4} = {30 \choose 26} = \frac{30!}{(30-26)!\cdot 26!} \\ \\
\text{Pascal's Identity} \\
\text{When } n = n \text{ on 2 choose functions:} \\
{n \choose r} + {n \choose k} = {n + 1 \choose r > k\ ?\ r:k } \\
\text{Example: } {6 \choose 4} + {6 \choose 3} = {7 \choose 4}
\end{gather*}
$$
# Venn Diagrams
- Uses over lapping circles or other shapes to illustrate the relationships between two or more sets of items. 
	- Set diagrams or Logic diagrams
- A ***Set*** is a collection of items.
	- $n(A)$ refers to the number of items in set A
	- $n(a')$ refers to the number of items that are NOT in set A.
		- **Complement of A**
		$$
n(A') = \text{ total } - n(A)
		$$
- **Union** means all of the elements in **set A** ***OR*** **set B**. We use the symbol $\cup$  to represent union.
$$
\begin{gather*}
\text{Example: even numbers } \cup \text{ numbers greater than } 50 \\
\{x \text{ is even}\}\cup\{x > 50\}
\end{gather*}
$$
- **Intersection** when an element is a member of **BOTH** sets
	- An element in **A** ***AND*** **B**
	- We use the symbol $\cap$ to represent an intersection
	$$
	\begin{gather*}
	\text{Example: even numbers } \cap \text{ numbers greater than 50} \\
	\{x \text{ is even}\} \cap \{x > 50\}
	\end{gather*}
	$$
# Rule of Sum
$$
\begin{gather*}
\text{Rule of Sum for } n(A \text{ or } B): \\
A\cup B = n(A) + n(B) - n(A\cap B)
\end{gather*}
$$
# Mutually Exclusive Events
- There are scenarios when two events cannot happen at the same time. These are called **mutually exclusive** events.
# Pascal's Triangle
$$
\begin{gather*}
\begin{array}{c c c c c c c c c c c c c c c}
 &  &  &  &  &  &  & 1 &  &  &  &  &  &  & & \text{Row } 0 = 2^0 = 1\\
 &  &  &  &  &  & 1 &  & 1 &  &  &  &  &  &  & \text{Row } 1 = 2^1 = 2\\
 &  &  &  &  & 1 &  & 2 &  & 1 &  &  &  &  & & \text{Row } 2 = 2^2 = 4\\
 &  &  &  & 1 &  & 3 &  & 3 &  & 1 &  &  &  & & \text{Row } 3 = 2^3 = 8\\
 &  &  & 1 &  & 4 &  & 6 &  & 4 &  & 1 &  &  & & \ \text{Row } 4 = 2^4 = 16\\
 &  & 1 &  & 5 &  & 10 &  & 10 &  & 5 &  & 1 &  &  & \ \text{Row } 5 = 2^5 = 32\\
 & 1 &  & 6 &  & 15 &  & 20 &  & 15 &  & 6 &  & 1 & & \ \text{Row } 6 = 2^6 = 64\\
1 &  & 7 &  & 21 &  & 35 &  & 35 &  & 21 &  & 7 &  & 1 & \ \ \ \text{Row } 7 = 2^7 = 128
\end{array} \\ \\
\text {The sum of the numbers in row } n \text{ of pascal's triangle is } 2^n\\ \\
\text{Pascal's Triangle can also be written in terms of combinations:} \\
\renewcommand{\arraystretch}{1.6} % try 1.6–2.0 for more height

\begin{array}{c c c c c c c c c c c c c c c}

 &  &  &  &  &  &  & \displaystyle {0 \choose 0} &  &  &  &  &  &  & \\

 &  &  &  &  &  & \displaystyle {1 \choose 0} &  & \displaystyle {1 \choose 1} &  &  &  &  &  & \\

 &  &  &  &  & \displaystyle {2 \choose 0} &  & \displaystyle {2 \choose 1} &  & \displaystyle {2 \choose 2} &  &  &  &  & \\

 &  &  &  & \displaystyle {3 \choose 0} &  & \displaystyle {3 \choose 1} &  & \displaystyle {3 \choose 2} &  & \displaystyle {3 \choose 3} &  &  &  & \\

 &  &  & \displaystyle {4 \choose 0} &  & \displaystyle {4 \choose 1} &  & \displaystyle {4 \choose 2} &  & \displaystyle {4 \choose 3} &  & \displaystyle {4 \choose 4} &  &  & \\

 &  & \displaystyle {5 \choose 0} &  & \displaystyle {5 \choose 1} &  & \displaystyle {5 \choose 2} &  & \displaystyle {5 \choose 3} &  & \displaystyle {5 \choose 4} &  & \displaystyle {5 \choose 5} &  & \\

 & \displaystyle {6 \choose 0} &  & \displaystyle {6 \choose 1} &  & \displaystyle {6 \choose 2} &  & \displaystyle {6 \choose 3} &  & \displaystyle {6 \choose 4} &  & \displaystyle {6 \choose 5} &  & \displaystyle {6 \choose 6} & \\

\displaystyle {7 \choose 0} &  & \displaystyle {7 \choose 1} &  & \displaystyle {7 \choose 2} &  & \displaystyle {7 \choose 3} &  & \displaystyle {7 \choose 4} &  & \displaystyle {7 \choose 5} &  & \displaystyle {7 \choose 6} &  & \displaystyle {7 \choose 7}

\end{array}
\end{gather*}
$$
- A set with $n$ distinct elements has $2^n$ subsets including the null set. The total number of combinations containing **at least one** item chosen from a group of $n$ distinct objects is $2^n-1$ 
- When solving for how many ways you can get to a location there is a shortcut you can use using:
$$
\begin{gather*}
\text{Paths } = \binom{x+y}{x \text{ OR } y} = \binom{x+y}{x} = \binom{x+y}{y}
\end{gather*}
$$

# Unit 1 Flashcards

#flashcards/School/Data/Unit-1/Terms-to-Definitions

What are **Independent Events**?
?
Events that have no effect on each other's outcomes. The probability of one event occurring does not influence the probability of the other event occurring.
<br>
*Example: When rolling a die and flipping a coin, the outcome of the die roll does not affect the outcome of the coin flip.*

***

How do you calculate the number of possible paths for independent events?
?
Multiply the number of possibilities for each event.
$$ 
\text{Possible Paths: } m \cdot n
$$ 
*m* and *n* are the number of possibilities for each event.
<br>
*Example: If you have 3 shirts and 4 pairs of pants, you have 3 * 4 = 12 possible outfits.*

***

How do you calculate the number of ways to arrange people around a round table?
?
The number of arrangements is (n-1)!, where n is the number of people.
<br>
*Example: 5 people can be seated in (5-1)! = 4! = 24 different ways around a circular table.*

***

What is **Factorial Notation**?
?
A way to represent the product of all positive integers up to a given number, *n*. It is written as *n*!
$$ n! = n \cdot (n-1) \cdot (n-2) \cdots 3 \cdot 2 \cdot 1 $$ 
<br>
*Example: 5! = 5 * 4 * 3 * 2 * 1 = 120*

***

How do you calculate arrangements with repeated elements?
?
For *n* objects, where *a*, *b*, *c*, etc., are the counts of each repeated element, the formula is:
$$ \frac{n!}{a!b!c!} $$ 
<br>
*Example: For the word "MISSISSIPPI", there are 11 letters total, with 4 'I's, 4 'S's, and 2 'P's. The number of unique arrangements is 11! / (4! * 4! * 2!) = 34,650.*

***

What is a **Permutation**?
?
An arrangement of items in a definite order, where the position is important.
<br>
*Example: The permutations of the letters A, B, C are ABC, ACB, BAC, BCA, CAB, CBA. The order matters.*

***

How do you calculate the number of permutations?
?
The number of arrangements of *n* objects taken *k* at a time is given by the formula:
$$ {}_nP_k=\frac{n!}{(n-k)!} $$ 
<br>
*Example: The number of ways to arrange 3 books from a collection of 5 is 5P3 = 5! / (5-3)! = 60.*

***

What is a **Combination** (Choose Function)?
?
A collection of chosen items where the order is not important.
<br>
*Example: Choosing 3 fruits from a basket of apples, oranges, and bananas. The group {apple, orange, banana} is the same as {banana, orange, apple}.*

***

How do you calculate the number of combinations?
?
The number of ways to choose *r* objects from a group of *n* objects is given by the formula:
$$ {n \choose r} = \frac{n!}{(n-r)!\cdot r!} $$ 
<br>
*Example: The number of ways to choose 2 students from a group of 5 is 5C2 = 5! / ((5-2)! * 2!) = 10.*

***

What is a **Venn Diagram**?
?
A diagram that uses overlapping circles to illustrate the relationships between two or more sets of items.

***

What is the **Union** of sets?
?
The set of all elements that are in **set A** OR **set B**. It is represented by the symbol $\cup$.
<br>
*Example: If Set A = {1, 2, 3} and Set B = {3, 4, 5}, then A $\cup$ B = {1, 2, 3, 4, 5}.*

***

What is the **Intersection** of sets?
?
The set of all elements that are in **BOTH** **set A** AND **set B**. It is represented by the symbol $\cap$.
<br>
*Example: If Set A = {1, 2, 3} and Set B = {3, 4, 5}, then A $\cap$ B = {3}.*

***

What is the **Rule of Sum**?
?
A formula to find the total number of elements in the union of two sets:
$$ n(A\cup B) = n(A) + n(B) - n(A\cap B) $$ 
It accounts for the elements that are in both sets so they are not counted twice.

***

What are **Mutually Exclusive Events**?
?
Events that cannot happen at the same time. The occurrence of one event prevents the other from occurring.
<br>
*Example: When flipping a coin, the outcomes of heads and tails are mutually exclusive.*

***

What is **Pascal's Triangle**?
?
A triangular array of numbers where each number is the sum of the two numbers directly above it. It is used in probability and combinatorics.

***

What is the relationship between Pascal's Triangle and combinations?
?
Each entry in Pascal's Triangle corresponds to a combination value ${n \choose r}$, where *n* is the row number (starting from 0) and *r* is the position in the row (starting from 0).
<br>
*Example: The number 6 in the 4th row of Pascal's Triangle is equal to ${4 \choose 2}$.*

***

How do you find the sum of the numbers in any row of Pascal's Triangle?
?
The sum of the numbers in row *n* of Pascal's Triangle is $2^n$.
<br>
*Example: The sum of the numbers in row 3 (1, 3, 3, 1) is $1+3+3+1 = 8$, which is equal to $2^3$.*
m



# Probability
- The measure of the likelihood of an event occurring
	- Fraction 
	- Decimal, range = $0\to 1$
	- Percent, range = $0\to 100\%$
	$$
	\begin{gather*}
	0 = \text{ impossible Event} \\
	\text{Example: } 2 + 2 = 5 \\ \\
	1= \text{ certain event} \\
	\text{Example: } 2+2=4
	\end{gather*}
	$$
# Theoretical Probability
- Predicting or estimated based on the possible number of outcomes
- No experiment if performed - based on reason and math
- Example:
	- Flipping a coin - we know its 50% without doing it
	$$
	\begin{gather*}
	\text{Sample Space = all outcomes that are possbile for and event } \to S \\
	n(S) = \text{Number of items in sample space (\# of outcomes)} \\ \\
	\text{Event Space } (A) \text{ - all outcomes that are considered "desired"} \\
	n(A) = \text{ the number of items in the event space} \\ \\
	\text{Theoretical Propability (if all the events are equally likely):} \\
	P(A) = \frac{n(A)}{n(S)} \\ \\
	\text{Sum of probabilities} \\
	\text{The sum of the probabilties of all the possible outcomes is } 1 \text{ or } 100\%
	\end{gather*}
	$$
# Experimental Probability
* Calculating probability based on an actual experiment
$$
\begin{gather*}
P(A) = \frac{\text{\# of times } A \text{ ocured}}{\text{\# of trials}}
\end{gather*}
$$
# Working With Probability
## Compliment
* to get the opposite probability of an even you can use complement
$$
\begin{gather*}
\text{The probability } A \text{ doesnt occur is: } \\
P(A') = 1 - P(A)
\end{gather*}
$$

## Multiplicative Property
$$
\begin{gather*}
\text{For two independent events } A \text{ and } B \text{:} \\
P(A\cap B) = P(A) \cdot P(B) \\ \\

\text{For two dependent events} A \text{ and } B \text{:} \\
P(A\cap B) = P(A) \cdot P(B|A)
\end{gather*}
$$
### Independent vs Dependent
* $A\cap B$ are **Independent** if the probability of one event doesn't affect the probability of the other 
* $A\cap B$ are **Dependent** if one of the events occurring affect the probability to change

### Conditional Probability
- The probability of an event **Given** that another event has **already** occurred \[$P(B|A)$\]
- ***NOT Mutually Exclusive***
- $P(A)>0$ 
$$
\begin{gather*}
P(B|A) = \frac{P(A\cap B)}{P(A)} \\ \\
\therefore P(A\cap B) = P(A) \cdot P(B|A)
\end{gather*}
$$


## Rule of Sum
$$
P(A\cup B) = P(A) + P(B) - P(A\cap B)
$$
### Mutually Exclusive vs Non-Mutually Exclusive
- **Non-Mutually Exclusive Events** can occur at the ***Same Time***$$
\begin{gather*}
P(A\cap B) \ne 0 \\
\therefore P(A\cup B) = P(A) + P(B) - P(A\cap B)
\end{gather*}
   $$
- **Mutually Exclusive Events** can ***NOT*** occur at the same time$$
	\begin{gather*}
P(A\cap B) = 0 \\
\therefore P(A\cup B) = P(A) + P(B)
\end{gather*}
	$$
## Probability Diagrams
* Probability trees can be used to organize our thinking if there are multiple cases to consider.
* Add the probability of each branch
```tikz

```
```tikz
````
```tikz
````
```tikz
````
```tikz
\begin{document}
\begin{tikzpicture}[x=10mm, y=10mm, font=\small]
% --- Nodes ---
\node (S) at (0,0) {Start};

\node (A)   at (3,  1.5) {$A$};
\node (nA)  at (3, -1.5) {$\overline{A}$};

\node (AB)    at (7,  2.5) {$A \cap B$\\ \scriptsize $P(A \cap B) = P(A)\,P(B \mid A)$};
\node (ABbar) at (7,  0.5) {$A \cap \overline{B}$\\ \scriptsize $P(A \cap \overline{B}) = P(A)\,P(\overline{B} \mid A)$};
\node (AbarB) at (7, -0.5) {$\overline{A} \cap B$\\ \scriptsize $P(\overline{A} \cap B) = P(\overline{A})\,P(B \mid \overline{A})$};
\node (AbarBbar) at (7, -2.5) {$\overline{A} \cap \overline{B}$\\ \scriptsize $P(\overline{A} \cap \overline{B}) = P(\overline{A})\,P(\overline{B} \mid \overline{A})$};

% --- Edges with probability labels ---
\draw[-latex] (S) -- (A)   node[midway, above] {$P(A)$};
\draw[-latex] (S) -- (nA)  node[midway, below] {$P(\overline{A}) = 1 - P(A)$};

\draw[-latex] (A)  -- (AB)     node[midway, above] {$P(B \mid A)$};
\draw[-latex] (A)  -- (ABbar)  node[midway, below] {$P(\overline{B} \mid A)$};

\draw[-latex] (nA) -- (AbarB)   node[midway, above] {$P(B \mid \overline{A})$};
\draw[-latex] (nA) -- (AbarBbar) node[midway, below] {$P(\overline{B} \mid \overline{A})$};
\end{tikzpicture}
\end{document}
```




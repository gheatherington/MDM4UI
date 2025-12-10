# Independent vs Dependent 
### Independent Variable
- Arbitrarily chosen
- On the $x$-axis
## Dependent Variable
- "Depends" on the Independent Variable
- On the $y$-axis

# Scatter Plots
- Visual (Graph) method of showing $2$ variable data
- Each point on graph represents a pair of values

## Types of Trends

![[Types of Trends.png]]
### Positive Correlation
- As the independent variable increases
- The dependent variable also increases
### Negative Correlation
- As the independent variable increases
- The Dependent variable decreases
### No Correlation
- There's no obvious relationship between the independent and dependent variables
## Types of Correlation
- It is normal to have a combinations of the Strong & Weak and Linear & Non-Linear quantifiers
- **Note:** if a correlation is non-linear, it may not be strictly increasing/decreasing

![[Types of Correlation.png]]
### Strong vs Weak
#### Strong Correlation
- Points form (or come close to forming) a line
#### Weak Correlation
- The correlation becomes weaker as points get further from forming a line
- Or further from the line of best fit

![[Strong vs Weak Correlation.png]]

### Linear vs Non-Linear
#### Linear Correlation
- When the points lie close to a straight line (line of best fit)
#### Non-Linear Correlation
- When the points are not well represented by a straight line
- But do lie close to a curve, called:
	- **The curve of best fit**

![[Linear vs Non-Linear Correlation.png]]

# Regression
- The process of fitting a line or a curve of best fit to a set of data
- Then determining the equation
- The equation for the line of best fit can used to make prediction based off the data

## Slope of Equation
- The slope of the regression equation can tell us the change in the dependent variable per unit increase of the independent variable
## $y$-Intercept
- The value of the dependent variable when the independent is at $0$

# Correlation Coefficient ($r$)
$$
\begin{gather}
r=\frac{\sum(x_i - \bar{x})(y_i-\bar{y})}{\sqrt{\sum(x_i-\bar{x})^2\sum(y_i-\bar{y})^2}} \\ \\
-1 \le r \le 1 \\
\text{As } |r| \to 1, \text{ the \textcolor{lightblue}{stronger} the correlation} \\
\text{As } |r| \to 0, \text{ the \textcolor{lightblue}{weaker} the correlation} \\ \\

\begin{array}{|c|c|c|c|}
\hline
\text{Strong} & \text{Moderate} & \text{Weak} & \text{No Correlation} \\ \hline
0.7\to1 & 0.5\to0.7 & 0.3\to5 & 0\to0.3 \\
\hline
\end{array}
\end{gather}
$$
- Measures the strength and direction of a linear correlation between two variables.
- A number that ranges between $-1$ and $1$ 
- The sign of the $r$-value indicates if the correlation is negative or positive

# Coefficient of Determination ($r^2$)
$$
\begin{gather}
r^2 = (r)^2= \left(\frac{\sum(x_i - \bar{x})(y_i-\bar{y})}{\sqrt{\sum(x_i-\bar{x})^2\sum(y_i-\bar{y})^2}}\right)^2 \\ \\
0 \le r^2 \le 1 \\
\text{As } r^2 \to 1, \text{ the better the fit of the trend line/curve}
\end{gather}
$$

- Represents how well the trend line represents the data
- Acts as a percentage of how many data points match with the trend line

# Residuals
$$
\begin{gather}
R = y_1 - (mx_1 + b); \text{ where,} \\ \\
\begin{aligned}
(x_1, y_1) & \to\text{ is a point in the data set} \\
m &\to\text{ is the slope of the trend line} \\
b &\to\text{ is the } y \text{-intercept of trend line}
\end{aligned}
\end{gather}
$$

- Often used to identify outliers
- They are the vertical distance between a point and the line (or curve) of best fit
- They are made up of 2 parts
	- The sign ($\pm$ positive/negative) indicated if it is above or below the trend line
	- And the magnitude of the distance
- A residual of $0$ means it lies directly on the trend line

## Residual Plot
- Residuals should be graphed so you can easily see the distances of each point from the line of best fit.

### Good Residual Plot
- If the model is a good fit, the residuals should be fairly small and there should be no noticeable pattern. 
- If all of the residuals are large or a noticeable pattern emerges, another model may be more appropriate.
![[Good Residual Plot.png]]

### Incorrect Slope
- There should be points above and below the $0$ line for all $x$-values shown
- Not the first half under the second half over

![[Incorrect Slop.png]]

### Incorrect Model
- In this example residuals form a parabola meaning our data is not linear
- A non-linear trend line would be more appropriate
![[Incorrect Model.png]]
# Outliers
- An **Outlier** is a point that is significantly different from the rest of the distribution
- Significantly further from the line of best fit than the other points
- An outlier is a point whose residual is significantly further from 0 compared to the other residuals.
- The point with the residual furthest from zero is not necessarily an outlier - there are sets of data with no outliers.
## Calculating Outliers
$$
\begin{gather}
\text{Outliers: } 
R(x) \lt -2\sigma \text{ OR }
R(x) \gt 2\sigma \\
\sigma = \sqrt{\frac{1}{N}\sum_{i=1}^{N}(x_i - \mu)^2}
\end{gather}
$$
# Influential Point
- A type of point that greatly affects the direction/slope of the line of best fit
- ***Often*** have large horizontal gaps between the point and the others
- They may have **small residuals** and therefore do **NOT** show up as **outliers**

![[Influential Point.png]]

## What to do with Influential Points
- Remove any outliers or influential points and recalculate:
	- correlation coefficient
	- and line of best fit
- Then compare the original vs without these points
- If they had a significant impact:
	- Investigate the points further
	- and discuss them in your findings
- You **CAN'T** pretend like they don't exist

# Types of Relations
- If there is a correlation between two variables, there are $3$ types of relationships that can exist
## Common Cause
- A $3$rd factor that exists that causes both variables to react
- **Example:** 
	- “In a growing municipality, the traffic planner observed that over a period of ten years the number of traffic accidents showed a high positive correlation with the number of traffic lights installed.”
	- **Common Cause:** More cars on roads

## Accidental Correlation 
- Sometimes the correlation is purely coincidental
- **Example:**
	- "With a decrease in the number of pirates we have seen an increase in global warming over the same time period."
	- Pirates $\ne$ Global Warming

## Cause and Effect (A Causes B)
- Where one variable does actually cause the behaviour of the other
- **Causation** v.s. Correlation
- **Example:**
	- "The more often you smoke and the longer you smoke, the greater your risk of lung cancer."
	- Therefore, smoking causes lung cancer.

# Misleading with Two Variable Data
- Implying causation based on correlation
- Making claims on a weak correlation
- Using $2$ different scales for $2$ different variables

# Spread Sheet
- Correlation Coefficient ($r$-value) $=\text{CORREL}(x_1:y_1, x_2:y_2$); where,
	- $x_1:y_1$ is the first column of the data
	-  $x_2:y_2$ is the second column of the data

# One Variable Data
## Measures of Central Tendency
- A measure of central tendency summarizes a set of numerical data using one value
- This value describes the centre of the data set
### Mean
- The average of the data set
- $\bar{x}$ for sample mean
- $\mu$ for population mean
$$
\begin{gather*}
\bar{x} = \frac{x_1 + x_2 + \ldots + x_n}{n}
\end{gather*}
$$
#### Weighted Mean
- A weighting can be applied to each mean
### Median
- The middle number when the data is ordered from lowest to highest (or highest to lowest)
- If there is an even number of values, use the average of the two middle numbers
$$
\begin{gather*}
\frac{n+1}{2}
\end{gather*}
$$

### Mode
- The value that occurs most often (highest frequency)
- There can be **NO** mode if they all occur **ONCE**
- Or multiple if there is a tie

## Grouped Data
- How do you calculate the mean, median and mode for data that is grouped in a frequency table
### Mode
- Choose the interval with the highest frequency

### Median
- Use of the following
$$
\frac{n+1}{2} \text{, where } n \text{ the total frequency (number of resposnes)}
$$

### Mean
- Get the mid points of each interval
- Multiple the midpoints by the number of frequency
- Divide the total products by the total frequency
## Outlier
- An element of data that is very different from the rest
- Can be multiple pieces of data (not just one)

### Position of Mean, Median, Mode
![[Position of Mean Media and Mode.png]]


$$
\begin{array}{|c|c|c|}
\text{Mean} & \text{Median} & \text{Mode} \\
\hline
\text{Moves with skew} & \text{Stays at ceneter} & \text{Stays at the peak} \\
& \text{(Best for central tendancy)} &
\end{array}
$$

#### Which to use
- If there is an outlier and/or your data is skewed use the **Median**
- If the data is **symmetric** use either **Mean** or **Median** (should be the same)
- if the data is qualitative (categorical) use **Mode**

## Types of Distributions
### Symmetric Distributions
- **Uniform** - all approximately the same height
  ![[Uniform Bar Graph.png]]
- **Mound** - peaks in the middle and tapers off to both sides
	- **NOTE:** *NOT* normal - normal has very specific specifications
  ![[Mount Bar Graph.png]]
- **U-Shaped** or **Bi-Modal**
	- Peak on Left and Right
	- Drops low in the middle
  ![[Bi-Modal Bar Graph.png]]

### Non-Symmetric Distributions

**Skew is the side of the decline**

- **Right/Positive** Skew
  ![[Positive Skew Bar Graph.png]]
- **Left/Negative** Skew
  ![[Negative Skew Bar Graph.png]]

## Displaying One Variable Data
- Use a **Histogram** to display continuous, numerical data
	- Money is always continuous
	- The interval size is also known as the **Bin Width** or **Bucket Size** (google sheets) and must be customized for each set of data.
- Use a **Bar Graph (Column Graph)** to display discrete, numerical data
	- Shoe sizes are discrete (even if its 7.5 for example)
	- OR Pie Chart - but only Bar Graphs are really used in this unit
### Reminders
- You need 5-10 bars
- **Interval** should be a nice easy number
- Avoid having spaces in the middle of the graph
- To create a histogram in Google Sheets, data must be **Unorganized**
- Data **HAS** to be **Organized** to create a bar graph

### Determining a Good Bin Width
$$
\begin{gather*}
\text{Upper Bound} = \frac{\text{Max Value} - \text{Min Value}}{\text{Min \# of Bars (5)}} \\
\text{Lower Bound} = \frac{\text{Max Value} - \text{Min Value}}{\text{Max \# of Bars (10)}} \\ \ \\
\text{Bin Width} = \text{Lower Bound} \le x \le \text{Upper Bound, } \\
\text{Where } x \text{ is a nice number} \\ \ \\
\text{Example:} \\
5, 18, 21, 23, 25, 36, 37, 42, 50, 50, 53, 54, 55, 61, 62, 70, 89, 91, 95, 99 \\ \ \\
\Delta = 99 -5 \\
\begin{array}{|c|c|}
\hline
\frac{94}{5} = 18.8 & \frac{94}{10} = 9.4 \\
\hline
\end{array} \\
\text{Bin Width should be between } 9.4 \text{ and } 18.8 \\
\therefore \text{ you could use 10 or 15}
\end{gather*}
$$
## Percentile
- The percent of data that are less than (or equal to) a specific data value.
	- You can argue either way; $\le$ or just $\lt$ 
- There are $2$-Formulas for percentiles. for both formulas your data must be arranged in order from smallest to largest.
### Formula \#1 
$$
\begin{gather*}
R = P(n+1)
\end{gather*}
$$
- Used to find what data value corresponds to a given percentile, where
	- $P$ is the percentile (in decimal form)
	- $n$ is the number of values
	- $R$ is the whole number "rank" of the data point.
- If you get a decimal value, take the average of the 2 points on either side
#### **Example** 
- Find the $80^{th}$ percentile and the $40^{th}$ percentile of the data set below
$$
\begin{gather*}
5, 18, 21, 23, 25, 36, 37, 42, 50, 50, 53, 54, 55, 61, 62, 70, 89, 91, 95, 99 \\ \ \\
\text{For } 80^{th}: \\
\begin{aligned}
R &= 0.80(20 + 1) \\
&= 16.8
\end{aligned}
\Rightarrow \text{ Average } 16^{th} \text{ and } 17^{th} \text{ data value} \\
\frac{70 + 89}{2} = 79.5 \\ \ \\
\text{For } 40^{th}: \\
\begin{aligned}
R &= 0.40(20 + 1) \\
&= 8.4
\end{aligned}
\ \Rightarrow 8^{th} \ \& \ 9^{th} \\
\frac{42 + 50}{2} = \boxed{46}
\end{gather*}
$$
### Formula \#2
$$
p = 100(\frac{L + 0.5E}{n})
$$
- To find what percentile a given data value is sitting at, where
	- $L$ is the number of data values lower than your point
	- $E$ is the number of data values equal to your point
	- $n$ is the number of data
	- $p$ is the percentile
- **NOTE:** Round to a whole number
#### **Example** 
- In the data set below, what percentile is the data value of $50$? And $91$?
$$
\begin{gather*}
5, 18, 21, 23, 25, 36, 37, 42, 50, 50, 53, 54, 55, 61, 62, 70, 89, 91, 95, 99 \\ \ \\
\text{For 50:} \\
p = 100(\frac{8 + 0.5(2)}{20}) = \boxed{45} \\
\therefore \text{ a score of } 50 \text{ is at a } 45^{th} \text{ percentile} \\ \ \\
\text{For 91:} \\
p = 100(\frac{17 + 0.5(1)}{20}) = \boxed{87.5} \\
\therefore \text{ a score of } 91 \text{ is at the } 88^{th} \text{ percentile}
\end{gather*}
$$
## Measures of Spread
- Measures of spread tell us whether our data are all very similar and clustered around the mean/median or whether there is a lot of variety in the data and the values are actually quite spread out.

### Range
$$
\begin{gather*}
\text{Range} = \text{Max} - \text{Min}
\end{gather*}
$$

### Quartiles
- Quartiles are three points that divide the data set into four equal groups.
	-  Q1 is the $25^{th}$ percentile
	- Q2 is the $50^{th}$ percentile
	- Q3 is the $75^{th}$ percentile
- Finding by Hand:
	- Arrange the data from smallest to highest
	- Find the median which is your Q2 ($50^{th}$ Percentile)
	- Then find the exact middle on either side of the median
#### Interquartile Range
- The interquartile range is the difference between the 3rd quartile and 1st quartile.
- The IQR is a better measure of spread than the range because it is not as affected by outliers. It only looks at the $50\%$ of the data in the middle of the data set.
$$
\begin{gather*}
\text{IQR} = \text{Q3} - \text{Q1}
\end{gather*}
$$
## Standard Deviation
- Standard deviation ($\sigma$) is a measure of the general distance between data points and the mean. It is a very reliable measure of spread.
$$
\begin{gather*}
\sigma = \sqrt{\frac{1}{N}\sum_{i=1}^{N}(x_i - \mu)^2} \\ \ \\
\text{Where} \\
\mu = \bar x  = \text{mean}\\
\sigma^2 = \text{varience} \\ 
\sigma = \text{standard deviation}

\end{gather*}
$$
Steps:
1. Find the mean for the data set
2. Subtract the mean from each individual data point
3. Square each difference from step $2$
4. Add all of the values from step $3$
5. Divide the sum from step $4$ by the number pf data values
6. Take the square root of your answer from step $5$ 

## Relative Deviation
- Compares the regular standard deviation against the mean of your data set
- Shows the amount of spread as a percentage
$$
\begin{gather*}
\text{RSD} = \frac{\sigma}{|\bar{x}|} \cdot 100\% = \frac{\sigma}{|\mu|} \cdot 100\% \\ 
\text{RSD} = \frac{\sqrt{\frac{1}{N}\sum_{i=1}^{N}(x_i - \mu)^2}}{|\mu|}
\end{gather*}
$$
- It’s generally reported to one or two decimal places and often converted to a percent. As the denominator is the absolute value of the mean, the RSD will always be positive.
- The higher the relative standard deviation, the more spread out the results are from the mean and the lower the relative standard deviation, the more closely the data is clustered around the mean.
- Particularly useful when comparing data sets and when working with data sets that have extremely large or extremely small data values.

## Identifying Outliers
- An outlier is identified as being more than $1.5$ times the $\text{IRQ}$ below Q1 or above Q3
$$
\begin{gather*}
x < (\text{Q1} - 1.5\cdot \text{IQR}) \Rightarrow x \text{ is an outlier} \\
x > (\text{Q3} + 1.5\cdot \text{IQR}) \Rightarrow x \text{ is an outlier}
\end{gather*}
$$
## Confidence Intervals
- Indication of how accurate estimate about population parameter is from the sample
- A range where the parameter would fall within

$$
\begin{gather*}
\text{MoE} = \pm Z(\frac{\sigma}{\sqrt{n}}) \\ \\
Z \text{ is the z-score}
\end{gather*}
$$

## Spreadsheet
- Mean $=\text{AVERAGE}(x:y)$
- Median $=\text{MEDIAN}(x:y)$
- Mode $=\text{MODE.MULT}(x:y)$
- Percentile $=\text{PERCENTILE}(x:y, z)$, where:
	- $x:y$ is the range
	- $z$ is the percentile as a decimal
		- For example for the $80^{th}$ percentile $=\text{PERCENTILE}(A1:A10, 0.8)$
- Range $=\text{MAX}(x:y)-\text{MIN}(x:y)$ 
- Quartiles $=\text{QUARTILE}(x:y, z)$ , where:
	- $x:y$ is the range
	- $z$ is the quartile you want ($1, 2, 3$)
		- For example: 1st Quartile $=\text{QUARTILE}(B1:A10, 1)$ 
- IQR $=\text{QUARTILE}(x:y, 3) - \text{QUARTILE}(x:y, 1)$ 
- Standard Deviation $=\text{STDEVP}(x:y)$ or $=\text{STDEV.P}(x:y)$ 
	- The formulas are different for population standard deviation and sample deviation are different
	- ONLY use **population** formula
- Margin of Error $=\text{CONFIDENCE.T}(1-p, \sigma, n)$, where:
	- $p$ is the confidence level
	- $\sigma$ is the standard Deviation 
	- $n$ is the number of trials

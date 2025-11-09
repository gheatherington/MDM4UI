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

### Mode
- The value that occurs most often (highest frequency)
- There can be **NO** mode if they all occur **ONCE**
- Or multiple if there is a tie

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


### Symmetric Distributions
- **Uniform** - all approximately the same height
  ![[Uniform Bar Graph.png]]
- **Mount** - peaks in the middle and tapers off to both sides
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
	- $p$ is the percentile (in decimal form)
	- $n$ is the number of values
	- $R$ is the whole number "rank" of the data point.
- If you get a decimal value, take the average of the 2 points on either side
**Example** 
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
**Example** 
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


## Spreadsheet
- Mean $=\text{AVERAGE}(x:y)$
- Median $=\text{MEDIAN}(x:y)$
- Mode $=\text{MODE.MULT}(x:y)$
- Percentile $=\text{PERCENTILE}(x:y, z)$, where:
	- $x:y$ is the range
	- $z$ is the percentile as a decimal
		- For example for the $80^{th}$ percentile $=\text{PERCENTILE}(A1:A10, 0.8)$

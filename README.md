# Descriptive-Statistics
Descriptive Statistics
Descriptive statistics are a set of techniques used to summarize or describe the main features of a dataset. They provide a simple and quick overview of the data and help to understand its central tendency, variability, and distribution. Descriptive statistics are essential for exploratory data analysis (EDA) and are often the first step in analyzing a dataset before applying more advanced statistical or machine learning techniques.

Key Concepts in Descriptive Statistics
Measures of Central Tendency: These statistics summarize the central point of a distribution of data.

Mean: The average of all values in the dataset.
Mean
=
1
𝑛
∑
𝑖
=
1
𝑛
𝑥
𝑖
Mean= 
n
1
​
  
i=1
∑
n
​
 x 
i
​
 
where 
𝑥
𝑖
x 
i
​
  represents each individual value in the dataset, and 
𝑛
n is the number of data points.
Median: The middle value of a dataset when arranged in ascending or descending order. If there is an even number of data points, it is the average of the two middle numbers.
Mode: The value that appears most frequently in the dataset. A dataset can have no mode, one mode, or more than one mode (bimodal, multimodal).
Measures of Variability (Spread): These statistics describe the dispersion or spread of data points in the dataset.

Range: The difference between the maximum and minimum values.
Range
=
Max
−
Min
Range=Max−Min
Variance: The average of the squared differences from the mean. It measures how spread out the values are in the dataset.
Variance
=
1
𝑛
∑
𝑖
=
1
𝑛
(
𝑥
𝑖
−
𝜇
)
2
Variance= 
n
1
​
  
i=1
∑
n
​
 (x 
i
​
 −μ) 
2
 
where 
𝜇
μ is the mean of the dataset.
Standard Deviation (SD): The square root of the variance. It gives a sense of how spread out the values are around the mean, and it is in the same units as the data.
Standard Deviation
=
Variance
Standard Deviation= 
Variance
​
 
Measures of Shape: These statistics describe the shape of the data distribution.

Skewness: Measures the asymmetry of the data distribution. A negative skew indicates that the left tail is longer, while a positive skew indicates that the right tail is longer. A skewness of 0 indicates a symmetric distribution.
Negative skew: Left tail is longer.
Positive skew: Right tail is longer.
Kurtosis: Measures the "tailedness" or the sharpness of the peak of a distribution. High kurtosis means more outliers, while low kurtosis indicates a flatter distribution compared to a normal distribution.
Position: These statistics describe the relative position of individual data points.

Percentiles: These are values below which a certain percentage of observations fall. For example:
25th percentile (Q1): The value below which 25% of the data falls (also called the first quartile).
50th percentile (Q2): The median.
75th percentile (Q3): The value below which 75% of the data falls (also called the third quartile).
Interquartile Range (IQR): The difference between the third quartile (Q3) and the first quartile (Q1). It represents the spread of the middle 50% of the data.
IQR
=
𝑄
3
−
𝑄
1
IQR=Q3−Q1
Descriptive Statistics in Practice
Let's walk through an example using a small dataset and calculate some of these key descriptive statistics.

Example Data (Monthly Sales):

Month	Sales
January	100
February	120
March	115
April	130
May	125
June	140
July	135
August	150
September	160
October	145
Step 1: Central Tendency
Mean (Average):

Mean
=
100
+
120
+
115
+
130
+
125
+
140
+
135
+
150
+
160
+
145
10
=
1370
10
=
137
Mean= 
10
100+120+115+130+125+140+135+150+160+145
​
 = 
10
1370
​
 =137
The mean sales for the year are 137.

Median: To find the median, we first sort the data: 
100
,
115
,
120
,
125
,
130
,
135
,
140
,
145
,
150
,
160
100,115,120,125,130,135,140,145,150,160 Since there are 10 data points, the median is the average of the 5th and 6th values:

Median
=
130
+
135
2
=
132.5
Median= 
2
130+135
​
 =132.5
Mode: There is no mode, as all values appear only once.

Step 2: Variability
Range:

Range
=
160
−
100
=
60
Range=160−100=60
The range of sales is 60.

Variance and Standard Deviation: To calculate the variance:

Variance
=
(
100
−
137
)
2
+
(
120
−
137
)
2
+
⋯
+
(
145
−
137
)
2
10
=
(
−
37
)
2
+
(
−
17
)
2
+
(
−
22
)
2
+
⋯
+
(
8
)
2
10
=
5868
10
=
586.8
Variance= 
10
(100−137) 
2
 +(120−137) 
2
 +⋯+(145−137) 
2
 
​
 = 
10
(−37) 
2
 +(−17) 
2
 +(−22) 
2
 +⋯+(8) 
2
 
​
 = 
10
5868
​
 =586.8
The variance is 586.8, and the standard deviation (square root of the variance) is:

Standard Deviation
=
586.8
≈
24.2
Standard Deviation= 
586.8
​
 ≈24.2
Step 3: Shape
Skewness: Skewness measures the symmetry of the data distribution. In this case, based on the values, it appears that the data is fairly symmetric, so the skewness would likely be close to 0 (you could calculate it precisely using software like Python or R).

Kurtosis: Kurtosis measures the peakedness of the distribution. You can compute it using statistical software, but intuitively, a value near 3 indicates a normal distribution.

Step 4: Position
Percentiles: To find the 25th percentile (Q1) and 75th percentile (Q3), we first sort the data: 
100
,
115
,
120
,
125
,
130
,
135
,
140
,
145
,
150
,
160
100,115,120,125,130,135,140,145,150,160
Q1 (25th percentile) is the 2.5th value, so:
𝑄
1
=
120
+
125
2
=
122.5
Q1= 
2
120+125
​
 =122.5
Q3 (75th percentile) is the 7.5th value, so:
𝑄
3
=
140
+
145
2
=
142.5
Q3= 
2
140+145
​
 =142.5
Interquartile Range (IQR):
IQR
=
𝑄
3
−
𝑄
1
=
142.5
−
122.5
=
20
IQR=Q3−Q1=142.5−122.5=20
The IQR is 20.
Summary of Descriptive Statistics for the Example:
Mean: 137
Median: 132.5
Mode: None
Range: 60
Variance: 586.8
Standard Deviation: 24.2
Skewness: Likely close to 0 (no extreme skew)
Kurtosis: Close to 3 (normal distribution)
Q1 (25th percentile): 122.5
Q3 (75th percentile): 142.5
Interquartile Range (IQR): 20
Descriptive Statistics in Python (Example)
Here’s how you can calculate these values using Python with pandas:

python
Copy code
import pandas as pd
import numpy as np

# Create the data
data = [100, 120, 115, 130, 125, 140, 135, 150, 160, 145]

# Convert to a pandas Series
series = pd.Series(data)

# Calculate descriptive statistics
mean = series.mean()
median = series.median()
mode = series.mode()[0]  # Returns the first mode value
range_value = series.max() - series.min()
variance = series.var()
std_dev = series.std()
q1 = series.quantile(0.25)
q3 = series.quantile(0.75)
iqr = q3 - q1

# Print the results
print(f"Mean: {mean}")
print(f"Median: {median}")
print(f"Mode: {mode}")
print(f"Range: {range_value}")
print(f"Variance: {variance}")
print(f"Standard Deviation: {std_dev}")
print(f"Q1 (25th percentile): {q1}")
print(f"




Continue generating





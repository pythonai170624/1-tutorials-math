# Statistical Distributions and Measures

## Distributions in Statistics

In statistics, a **distribution** refers to the arrangement or pattern in which data values are spread across different ranges or categories in a dataset. It provides an overview of how individual data points are distributed along a number line or within intervals.

### Types of Statistical Distributions

There are two main types of statistical distributions:

#### 1. Discrete Distribution
- The variable can take on only a finite number of values
- **Examples**: 
  - Rolling a die (results can only be between 1 and 6)
  - Number of calls at a call center (integer values only)

#### 2. Continuous Distribution
- The variable can take on infinite values or any value in a range
- **Examples**: 
  - Weights of individuals
  - Time taken to run a mile (these can be any real number)

### Common Probability Distributions

#### Uniform Distribution
- Each outcome has the same probability of occurrence
- **Examples**:
  - The `randint()` function in Python
  - Rolling a fair die where each number has the same probability (1/6)

#### Binomial Distribution
- Models the number of successes in a fixed number of Bernoulli trials
- A Bernoulli trial is an independent experiment with only two possible outcomes: "success" and "failure"
- **Example**: 
  - Flipping a coin multiple times and counting the number of "heads"

## Statistical Measures

### Mean (μ)

The mean, often referred to as the average, is a fundamental concept in statistics. It represents the arithmetic sum of all the values in a data set divided by the count of values in the dataset.

**Formula**: 
$$\mu = \frac{\sum X}{N}$$

Where:
- $\sum$ symbolizes the sum
- $X$ represents each value in the dataset
- $N$ is the total number of values

### Variance (σ²)

Variance is a statistical measurement that describes the spread of numbers in a dataset. It measures how far each number in the set is from the mean (average) and thus from every other number in the set.

**Formula**:
$$\sigma^2 = \frac{\sum(X - \mu)^2}{N}$$

Where:
- $\sigma^2$ is the variance
- $\sum$ symbolizes the sum
- $X$ represents each value in the dataset
- $\mu$ is the mean
- $N$ is the total number of values

### Standard Deviation (σ)

The standard deviation is a statistical measure that reflects the amount of variation or dispersion from the average (mean) in a data set. A low standard deviation indicates that the data points tend to be close to the mean, while a high standard deviation signifies that the data points are spread out over a wider range.

**Formula**:
$$\sigma = \sqrt{\frac{\sum(X - \mu)^2}{N}}$$

The standard deviation is simply the square root of the variance.

## Practical Example

Let's calculate the mean, standard deviation, and variance for this dataset: [5, 7, 11, 15, 18]

### Step 1: Calculate the Mean
$$\mu = \frac{5 + 7 + 11 + 15 + 18}{5} = \frac{56}{5} = 11.2$$

### Step 2: Calculate the Variance

Find each squared distance from the mean:
- $(5 - 11.2)^2 = (-6.2)^2 = 38.44$
- $(7 - 11.2)^2 = (-4.2)^2 = 17.64$
- $(11 - 11.2)^2 = (-0.2)^2 = 0.04$
- $(15 - 11.2)^2 = (3.8)^2 = 14.44$
- $(18 - 11.2)^2 = (6.8)^2 = 46.24$

Sum these squared differences and divide by the count:
$$\sigma^2 = \frac{38.44 + 17.64 + 0.04 + 14.44 + 46.24}{5} = \frac{116.8}{5} = 23.36$$

### Step 3: Calculate the Standard Deviation
$$\sigma = \sqrt{23.36} = 4.83$$

### Results:
- **Mean (μ)**: 11.2
- **Variance (σ²)**: 23.36
- **Standard Deviation (σ)**: 4.83

## Why These Measures Matter

- **Mean** provides the central tendency of the data
- **Variance** shows how spread out the data is from the mean
- **Standard Deviation** gives a measure of dispersion in the same units as the original data

These measures help us understand the characteristics of a dataset and make informed decisions based on the data's distribution.

# Terminologies

---

1. **_Data Science_**
   1. It is an interdisciplinary academic field that uses statistics, scientific computing, scientific methods, processes , algorithms and systems to extract or extrapolate knowledge and insights from noisy, structured and unstructured data
      1. Unstructured data = data make sense, but we can't pin point exact location to get particular information.
   2. is a "Concept to unify statistics, data analysis, machine learning and their related methods" in order to "understand and analyze actual phenomena" with data.
   3. ![What is Data Science](./datascience.png)
2. **_Why Data Science_** ?
   1. Businesses looking to use data to gain competitive advantage
   2. Technological advancements - data storage, processing power, clouse based storage and computing
   3. Burst in Data - Internet, electronic devices
   4. The ability to take data - to be able to understand it, to process it, to extract value from it, to visualize it, to communicate it - that's going to be ahugely important skill in the next decades. - Hal Varian.
3. **_What is Machine Learning ?_**
   1. Machine learning is a study of algorithms and statistical models that computer systems use in order to perform a specific taks effectively without being explicitly programmed, relying on patterns instead.
   2. ![[MachineLearning.png]](./MachineLearning.png)
   3. In libraries there are mathematical principles to generate equations for the given scenario
4. **_Artificial Intelligence vs Machine Learning vs Deep Learning_**
   1. Making machine intelliegent by any means
   2. Programs with the ability to learn and reason like humans
   3. There can be explicit programming (Rule based programs)
   4. Machine Learning
      1. Algorithms with the ability to learn without being explicitly programmed.
      2. Learn from pattern
   5. Deep Learning
      1. Subset of machine learning in which artificial neural networks adapt and learn from vast amounts of data
      2. Patterns drawn using neural network.
5. **_Uses of ML_**
   1. Data patterns are too complex and constantly changing. E.g. weather forecasting.
   2. We find it hard to express our knowledge about patterns as a program. e.g. Character recognition
   3. We do not readily have an algorithm to identify a particular pattern e.g. spam mail detection
   4.
6. **_Important Terms_**
   1. The value which we want to predict:
      1. Target variable, Dependant variable, Y, Predicted variable, Label
   2. The values using which we will attempt to predict:
      1. Features, Dimension, Independent Variables, Xs, Predictor variable
7. **_Classification_**
   1. Supervised Learning
      1. There is $Y$ to be predicted
      2. If $Y$ is a number i.e continuous variable then we call it as Regression
      3. If $Y$ is a category then it is called classification
   2. UnSupervised Learning
      1. There is no $Y$ to be predicted
      2. There is a logical group in data - cluster analysis - market segmentation
      3. Dimensionality Reduction
      4. Artificial Neural Network just needed linear algebra and metrics
8. **_Supervised Machine Learning_**
   1. ![[SupervisedLearning.png]]
9. ***Basic Statistics***
	1. The collection of all data points is the **population** or the **universe** data for a process
	2. A subset of points drawn from a population is called **sample**
	3. Measurement of a characteristic of sample is called **Statistic**
	4. Measurement of a characteristic of population is called **Parameter**
	5.  Types of Data
		1. Categorical - Preferred band
		2. Numeric
			1. Discrete - Number of items sold
			2. Continuous - Weight of a product
	6.  Measurement Scale
		1. Categorical (Qualitative)
			1. Nominal - doesn't have order(gender)
			2. Ordinal - has meaningful order(appraisal rating)
		2. Numeric(Quantitative)
			1. Interval - Temperature in Celsius
				1. ![[Pasted image 20230306142937.png]]
			2. Ratio - Cost of an item
	7.  **Descriptive Stats**
		1.  Central Tendency
			1. Mean: Arithmetic mean of numbers. Add the observations and divide by count of the observations. Mean is affected by extreme values.
			2. Median: When observations are sorted in the ascending order, the middle observation is median. If we have n observations, the (n + 1)/2 th obervation is median. The median can be an observation or between two observations.
			3.  Mode: Mode is the most frequently occuring data point in a data set.

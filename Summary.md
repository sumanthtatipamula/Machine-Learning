
## Terminologies

---

1. **_Data Science_**
   1. It is an interdisciplinary academic field that uses statistics, scientific computing, scientific methods, processes , algorithms and systems to extract or extrapolate knowledge and insights from noisy, structured and unstructured data
      1. Unstructured data = data make sense, but we can't pin point exact location to get particular information.
   2. is a "Concept to unify statistics, data analysis, machine learning and their related methods" in order to "understand and analyze actual phenomena" with data.
   3. ![What is Data Science](datascience.png)
2. **_Why Data Science_** ?
   1. Businesses looking to use data to gain competitive advantage
   2. Technological advancements - data storage, processing power, clouse based storage and computing
   3. Burst in Data - Internet, electronic devices
   4. The ability to take data - to be able to understand it, to process it, to extract value from it, to visualize it, to communicate it - that's going to be ahugely important skill in the next decades. - Hal Varian.
3. **_What is Machine Learning ?_**
   1. Machine learning is a study of algorithms and statistical models that computer systems use in order to perform a specific taks effectively without being explicitly programmed, relying on patterns instead.
   2. ![MachineLearning.png](MachineLearning.png)
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
   1. ![SupervisedLearning.png](images/SupervisedLearning.png)
9. **_Basic Statistics_**
   1. The collection of all data points is the **population** or the **universe** data for a process
   2. A subset of points drawn from a population is called **sample**
   3. Measurement of a characteristic of sample is called **Statistic**
   4. Measurement of a characteristic of population is called **Parameter**
   5. Types of Data
      1. Categorical - Preferred band
      2. Numeric
         1. Discrete - Number of items sold
         2. Continuous - Weight of a product
   6. Measurement Scale
      1. Categorical (Qualitative)
         1. Nominal - doesn't have order(gender)
         2. Ordinal - has meaningful order(appraisal rating)
      2. Numeric(Quantitative)
         1. Interval - Temperature in Celsius
            1. ![Numeric.png](Numeric.png)
         2. Ratio - Cost of an item
   7. **Descriptive Stats**
      1. <mark style="background: #FF5582A6;">Central Tendency</mark>
         1. <mark style="background: #FFF3A3A6;">Mean</mark>: Arithmetic mean of numbers. Add the observations and divide by count of the observations. Mean is affected by extreme values.
            1. Gets Influenced by the outliers
            2. Eg: Salaries : 9,12,10,11,8, 130 Lakhs because of the 1.3cr package mean doesn't provide accurate representation
         2. <mark style="background: #FFF3A3A6;">Median</mark>: When observations are sorted in the ascending order, the middle observation is median. If we have n observations, the (n + 1)/2 th obervation is median. The median can be an observation or between two observations.
         3. Mode: Mode is the most frequently occuring data point in a data set.
      2. <mark style="background: #FF5582A6;">Range</mark>: It is the difference between the maximum and minimum values in a data set. Affected by extreme values
         1. Very sensitive to outliers than mean
      3. <mark style="background: #FF5582A6;">Inter Quartile Range (IQR) </mark>??? IQR is the distance between the first and the third quartile.
         1. First quartile (Q1) has 25% observation lower than it.
         2. Third quartile (Q3) has 75% observation lower than it. $3 * (n + 1) / 4$
         3. Median is also called second quartile (Q2)
         4. Application of IQR will be finding outliers.
         5. Max length of whisker = 1.5 \* IQR
         6. ![IQR.png](IQR.png)
         7. Any point which is less than Q1 - Max Length Whisker or Q3 + Max Length Whisker is a Outlier
         8. Can be used to tell where points are densly packed
      4. Variance and Standard deviation
         1. Variance is measured as the average of sum of squared difference between each data point(represented by xi) and the mean represented by
            1. N - consistent formula
            2. N - 1 - unbiased formula
         2. Standard deviation is one of the most popular measure of spread. It is the square root of the variance.
         3. ![Symbols.png](Symbols.png)
      5. Normal Curve
         1. Outputs of a process vary due to various factors that come into play during the process
         2. Probability Distribution - Listing out all possible values along with their probabilities
            1. For continuous variables we can't list all values
               1. ![UniformDistribution.png](UniformDistribution.png)
               2. This graph is said to be uniform Distribution
            2. ![ProbabilityDistribution.png](ProbabilityDistribution.png)
         3. Area of the curve gives probability.
         4. Standard Normal Distribution is one where mean = 0 and standard deviation = 1
         5. ![NormalDistribution.png](NormalDistribution.png)
         6. Sampling Distribution of Mean and Central Limit Theorem
         7. Z tells how many standard deviation away from mean.
      6. Hypothesis Testing
         1. A hypothesis is an educated guess or proposition that attempts to explain a set of facts or natural phenomenon.
         2. ![TcketResolution.png](TcketResolution.png)
         3. ![Hypothesis.png](Hypothesis.png)


## libraries
1. [numpy](./Libraries/Numpy/Numpy.m)

## Algorithms

 ## Supervised Learning
	 ![[SupervisedLearning 2.png]]
	 1. Part of the data we givesome part for training and some part for testing. i.e 70 % to 80 % data will be going for training and 30 % to 20% rows will go for testing. The split is done randomly.
		 1. For all Classification algorithms we use Accuracy, Confusion Matrix, Precision , Recall, F1
		 2. For Regression = $R^{2}$
	 2. ***K Nearest Neighbors***
		 1. Commonly used for classification
		 2. Can also be used for regression
		 3. Classification is determined based on a majority vote of the nearest neighbors of each point
		 4. Though it is a supervised learning method, it is a ???lazy learner???, i.e. does not construct a model using training data.
		 5. Not suitable if the data is too noisy or the target classes do not have clear demarcation in terms of attribute values.
		 6. Suitable for classification where items in a class tend to be fairly homogenous on the values of attributes
		 7.  When classification is <mark style="background: #FF5582A6;">binary</mark> we can avoid tie by giving K an odd number.
			 1. ![KNN.png](KNN.png)
		 8.  Distance Calculations
			 1. Euclidean distance $= \sqrt{ (x_{2} - x_{1}) ^{2} + (y_{2} - y_{2})^{2} }$
			 2. Manhattan / Taxi Distance $=  | x_{2} - x_{1}| + |y_{2} - y_{1} |$
			 3.  Minkowski = $(| x_{2} - x_{1}|^{p} + |y_{2} - y_{1} |^{p} + \dots) ^{1 / p}$
				 1. p = 1 manhattan
				 2. p = 2 Euclidean
			 4. Mahalanobis distance
			 5. Matching Distance(for Boolean Data) = $\frac{number\  of\ non\  equal\  dimensions}{number\  of\  dimensions}$
		 9.  We need to bring data to common scale(using min-max or Z)
			 1. ![[KNN_Example1.png]]
			 2.  Here if we see the distance 1 and 3 are less so they appear to be similar but with domain knowledge 1 and 2 will be same as they have same age.
			 3. In these cases distances could lead incorrect results to avoid that we use standardisation (i.e columns data is in different scale)
				 1.  Z- score $=\frac{x_{i} - \bar{x} }{S}$
				 2.  Min - max scaler = $\frac{X - min}{max -min}$ values between will  be between 0 to 1
				 3.  After applying min - max scaler ![[min-max-scaler.png]]
				 4. scaler.fit_transform(x_train)
					 1. ![[FitTransform.png]]
					 2. For test we should never do fit_transform. only transform to be used and the mean and std dev will be used from Xtrain because we want neighbours for test to be same as of train.
				 5.  ![[knn_snippet.png]] Classifier.fit doesn't create any model. It just map X_train and Y_train
		 10.  <mark style="background: #FF5582A6;">Training Accuracy</mark> :  Testing train data for accuracy `classifier.score(X_train, y_train)`
			 1. Why Training accuracy may not be 100 % because in K neighbours 1 neighbour will be itself. so if we try with k = 1 accuracy will be 100 % because each row maps to one in trained(train == test) 
		 11. Confusion Matrix:
			 1. ![[ConfusionMatrix.png]] `metrics.confusion_matrix(y_test, y_predict)` `print(metrics.classification_report(y_test, y_predict))`
			 2. Classification accuracy = correct predictions / total predictions
			 3.  Precision is the proportion of the predicted positive cases that were correct.
				 1. Precision of C = 15 / (15+1)
				 2. Precision of B = 19 / 19
				 3. Precision of  A = 15 / 15
			 4. Recall is the proportion of positive cases that were correctly identified 
				 1. Recall for B = 19 / (19+1)
				 2. Recall for A,C = 15 / 15
			 5. F1 score = $\frac{2*(Recall * Precision)}{(Recall + Precision)}$
	 3. ***Linear Regression***
		 1. The term "linear" in the name ???linear regression??? refers to the fact that the method models data with linear combination of the explanatory (independent) variables.
		 2.  *Covariance*:
			 1. measures the join variability between two numerical variables (X and Y).
			 2. $Cov(x, y) = \frac{\sum{(x_{i} - \bar{x}) * (y_{i} - \bar{y})}}{n - 1}$
				 1. If Y increases with X then cov(x,y) > 0
				 2. If Y decreases with X then cov(x, y) > 0
			 3. Coefficient of correlation measures the strength of a linear relationship netween two variables (X and Y)
				 1. Value lies between -1 and 1
				 2.  $r = r_{{xy}} = \frac{Cov(x,y)}{S_{x} * S_{{y}}}$
				 3. ![[correlation.png]]
				 4. Practically +1 or -1 or 0 is impossible
				 5. Value nearer to -1 or 1 indicates stronger correlation 
		 3.  Linear regression fits a line to build a model. There are infinite number of lines that can be drawn through the training points. Which line should we consider as the model
			 1. The line with the least value total sum of squared prediction errors (in diagram shown as SSE) is considered as <mark style="background: #FFF3A3A6;">best fit line.</mark> This is called Cost Function or Loss Function = $\sum{(actual - predicted) ^{2}}$
			 2. Actual Y - Predicted Y is error
		 4. How equation of line is formed ![[BestFitLine.png]]
			 1. <mark style="background: #BBFABBA6;">Gradient Descent</mark>: Minimize SSE to determinre best fit line(b0, b1)
				 1. ![[GradientDescent.png]] it is not realistic because we didn't consider b1
				 2. ![[GradientDescentWithB1.png]]
		 5. Measuring Performance of Linear Equation
			 1. For linear regression the performance measurement is about how close to the actual prediction is.
			 2. The Sum of Squares Regression is the sum of the squared differences between the prediction for each observation and the population mean. = $= \sum{(predicted \ Y - Mean \ of\ Y)}^{2}$ 
			 3. The proportion of total variation (SST) that is explained by the regression (SSR) is known as the Coefficient of Determination.
				 1. $R^{2} = \frac{SSR}{SST}$
				 2. Value of R will lie between 0 and 1
				 3. ![[Linear_Regression_Performance.png]]
				 4. Coefficient of Determination (R2). Higher value of is R2 indicates better accuracy
			 4. Mean Squared Error (MSE). Lower value of MSE indicates better accuracy
					 1. $=  \frac{SSE}{n}$
			 5. RMSE = $\sqrt{ MSE }$
			 6. Mean Absolute Error $= \frac{\sum{Error}}{n}$
		 6.  If p > 0.05 the column is significant ![[hypothesis_LR.png]]
		 7. Training accuracy will always goes down if we remove any column whether it is useful or not.
			 1. Why even though it appears there is no correlation but in reality there will be cov > 0
				 1. ![[CovBetweenRandomNumbers.png]]
				 2. ![[LRTrainingAccuracy.png]]
		 8.  Scaling is not required because every column has it's own coefficient, the performance will not change with or without.
		 9. If multi collinearity exists then we need to use VIF, LASSO regression, PCA, Adjusted R-squared
	 4. ***Logistic Regression***
		 1.  It uses Sigmoic function to make probabilistic prediction. Probability P that a data point belongs to a class for a given value x =  $\frac{1}{1 + e^{-(b_{0} + b_{1} * x)}}$
		 2.  Probability Value lies between 0 and 1
		 3. By chaning $b_{0}$ curve will shift to its left($\uparrow$) or right with ($\downarrow$).
		 4. By changing $b_{1}$ curve becomes sharp($\uparrow$) and slant with ($\downarrow$).
		 5. So we need to achieve best fit curve by chaning $b_{0}$ and $b_{1}$.
		 6. Optimization for  equation of line
			 1. Maximise Likelihood =  $\prod^{1}_{n} p_{i}^{y_{{i}}} * (1 - p_{{i}} ^{(1 - y_{{i}})})$
				 1. ![[LRHeartProblem.png]]
				 2. Since P values lies between 0 and 1 product results in lots of Zeros to avoid that we use 
			 2.  Maximise Log(likelihood) = $\sum(y_{{i}}\log(P) + (1 - y_{{i}})* \log(1 - P))$
			 3.  Solving Min log loss gives best $b_{0}$ and $b_{1}$
			 4. If p(cutoff) >= 0.5 then predict Y = 1 else predict Y = 0. Cutoff can be changed manually.
		 7. Stratify = returns training and test subsets that have the same proportions of class labels as the input dataset.
			 1. Use it only for classification not for regression
		 8. Scaling is required for logistic regression becuase of Regularisation
	 5. ***Decision Tree or Classification And Regression Tree(CART)***
		 1. Returns training and test subsets that have the same proportions of class labels as the input dataset.
		 2. It is a greedy algorithm
		 3. Tree consistes of  Nodes and Branches
			 1. Nodes are decision points
				 1. Root Node: Representing Original Data
				 2. Branch Node: representing a decision function
				 3. Leaf Node : (holds the result of all previous functions that flow to it).
				 4. Pure Node : It is a leaf node with entropy 0
			 2. Branches are result of decision function
		 4. Algorithm:
			 1. Tree creation splits data into subsets and subsets into further smaller subsets.
			 2. The algorithm stops splitting data when data within the subsets are sufficiently homogenous or some other stopping criterion is met.
			 3. After executing all the decision functions from Root Node to Leaf Node, the class of a data point is decided by the leaf node to which it reaches. 
				 1. Then predict based on majority class.
		 5. Decision Tree algorithm learns through the measure of impurity of data in a node.
			 1. Entropy = $\sum^{1}_{c}(-p_{{i}} * log(p_{{i}}))$
			 2. Entropy ranges from 0 to 1
			 3. Entropy = 0 means 100% information
			 4. Entropy =  1 means maximum uncertainity or impurity
		 6. ![[DecisionTree1.png]]
			 1. Try all possible splits and select the one with highest information gain. i.e in above image split is done using age. now we need to try splitting using income,student etc. we select the split based on information gain. i.e whichever gives heghest information gain that is selected.
		 7. Gini Index is another measure which gives similar results as entropy $Gini = 1 - \sum^{i =  1}_{C}(p_{{i}}^{2})$
			 1. when uncertainity value will be 0.5 
			 2. In perfectly classifed node, values will be 0
		 8. We can use either gini or entropy, choose based on which one performs better.
		 9. In the above image decision tree has more than 2 children, but in actual decision  tree it should be only 2 children.
			 1. Categorical Variable Encoding
				 1. ![[CategoricalEncoding.png]]
				 2. First level Split ![[TreeConstructWithEncoding.png]]
				 3. ![[SplitonNumeric.png]]
		 10. More the info gain and more the records passing through it, more the importance `dt_model.feature_importances`
		 11. ![[DecisionTreeFit.png]]
		 12. Decision Tree Parameters
			 1. Max_Depth: Is the maximum length of a path from root to leaf. see above Image for reference
			 2. Min_Sample_Split : Before split check the number of records in a node.
				 1. ![[min_sample_split.png]]
			 3. Min_Sample_Leaf : After the split check the number of records in each child node.
				 1. ![[min_leaf_split.png]]
			 4. max_leaf_nodes = maximum number of leaf nodes in a tree.
			 5. **Hyper Parameter Tuning : Grid Search**
				 1. ![[HyperParameterTuning.png]] rows are splitted based on nfolds value
				 2. average is taken
	 6. ***Random Forest***
		 1. There is disadvantage with decision tree, they are too much sensitive to data.
		 2. *Ensemble Techniques*:
			 1. Build All possible and let them do prediction, whichever performs better we pick that.
			 2. Combining the outputs of several classifiers may reduce the risk of selecting a poorly performing Classifier
		 3. *Bootstrap Sampling*:
			 1. Generate new training sets using sampling with replacement. It is called bootstrap sampling.
			 2. Testing ![[bagging.png]]
		 4. ![[RandomForest.png]]
			 1. By default it picks random n ** 0.5, but it can be overridden.
	 7. ***Naive Bayes Classifier***
		 1. Its a pure classifier and can't be used in regression
		 2. It is based on Bayes theorem. It is called ???na??ve??? due to the assumption that the features in the dataset are independent which may not be true in the real world.
		 3.  Conditional Probability: it is the probability that an event given another event has occurred.
			 1. Given the card drawn is red. What is the probability it is an ace ? = 2 / 26
			 2.  $P\left(\frac{Ace}{Red}\right)= p(Ace \cap Red) / P(\mathrm{Re}d)$ 
			 3. $P(A \cap B) = P(A) * P(B)$ when A and B are independent
			 4. $P\left(\frac{A}{B}\right) = \frac{P\left(\frac{B}{A}\right)* P(A)}{P(B)}$ - Bayes Theorem
				 1. $P(A)$ is prior probability
				 2. $P(\frac{A}{B})$ - posterioir probability
			 5. ![[Bayes 1.png]]
			 6. ![[BayesProblem.png]]
			 7. ![[BayesProblemWithXContinuous.png]]
			 8. ![[BayesAlgorithms.png]]
		 4. Handling missing values
			 1. Delete the rows
			 2. Replace with mean/median/mode - done when only a few rows have missing values
			 3. Drop the column(if most of the values in the column are missing)
			 4. Get the missing data from another source(ideal which not happens in most of the cases).
			 5. Predict the missing values using other X's
			 6. Replace based on domain knowledge
	 8.  ***Support Vector Machine***
		 1. Comonly used for classification
		 2. It attempts to find Hyperplane, linearly seperating data. In low dimension space, it is a line: $w_{1}x_{1} + w_{2}x_{2} + b = 0$ where $x_{1}, x_{2}$ are features
		 3. Perceptron algorithm
			 1. Select random sample from training set as input
			 2. if classification is correct, do nothing
			 3. if classification is incorrect, modift the weight vector w
			 4. Reapeat the above two stesp until the entire training set is classfied correctly.
		 4. If the data is linearly separable then it will find the line/surface that linearly separate the data.
	 9. ***Artificial Neural networks***
		 1.  How manu neurons chosen in hidden layer is hyper parameter.
		 2. A random weight is assigned during initialization to each line except the final output.
		 3. Each neuron has input and a function that generates output.
		 4. Input recived by neuron is $\sum^{k = 1}_{n} I_{{k}}W_{{k}}$ W is random weight.
		 5. Bias Inputs is like $b_{0}$ in other algorithms
		 6.  for the result of the input we apply any of the three functions to generate output for current neuron and input to next level neuron.
			 1. Sigmoid
			 2. TanH
			 3. ReLU
		 7. The above 3 functions are called activation function and  it is a hyper parameter.
		 8. Selected activation funcion is applied to all hidden layer neurons.
		 9. How many hidden layers is also a hyper parameter.
		 10.  Output layer function
			 1. *for regression*: output activation function is identity = so what input it recieves same is the output.
			 2. *for binary classification* : activation function is sigmoid whose value lies between 0 and 1
			 3. *Multi class classfication*: (3 class)
			 4. ![[outputlayerneuron.png]]
			 5. ![[neuralnetworkfit.png]]
		 11. Perform as many epochs as possible till error is no longer reducing. 1 epoh is equivalent to one forward and one backward propagation.
		 12. Processing not done row by row of data set instead matrix multiplication is used
		 13. Stochastic Solvers
		 14. 
	 10. In classification Boosting
		 1. Ada Boost
		 2. GBM
		 3. XG Boost
	 11.  In clustering
		 1. BSCAN
	 12. Dimension Reduction
		 1. LDA
	 13. Time Series
	 14. Recommendation Engines
	 15. Reinforcement Learning

## Unsupervised learning
1.  Intro
	1. We are not interested in prediction. The model is not provided with the correct results during the training
	2. The goal is to discover interesting things about data
2. Clustering
	1. A technique to organize unlabeled data into similar subgroups. It is a techniques of discovering subgroups, or clusters, in a dataset.
	2. A good cluster shall have high 
		1. Intra-class similarity: Similarity between objects in same cluster 
		2. Inter-class dissimilarity: dissimilarity between objects in different clusters
	3. Types of clustering
		1. Hierarchical Clustering
		2. Partitioning Clustering
	4. K means Clustering
		1. It is a partitioning Clustering
		2. Widely used in Data mining
		3. K means no.of clusters and it is a hyper parameter.
		4. Algorithm:
			1. It is an iterative clustering algorithm
			2. Pick K random points as cluster centers(C1, C2, .. CK)
			3. Form K clusters by assigning all data points to closest centroid.
			4. Recompute centroid of each cluster
			5. Repeat above 2 steps until no points assignments change take place or fixed number of iterations.
		5. How to determine K 
			1. A simple strategy is to compute a clustering for various values of K and choose the best one.
			2. Measure the quality of a clustering by distance of points cluster centers. It is called Inertia in python.
			3. WCSS  vs K graph is called eblow plot or screen plot.
				1. Use elbow chart method to determine value of K where benefit doesn???t increase by ???much??? by increasing the value of K.
			4. **silhouette score**  - need ot be explored.
		6. How to determine initial centroid.
			1. Scikit-learn has implemented K-mean++ for initial centroid. It initializes centroids to be distant to one another which leads to better results for 10 times.
		7. Perform clustering using only meaningful columns(i.e based on subjective decision what we want to understand about data/ based on what characteristics we want to segment the customers).
		8. Typically done using numeric X's
	5. Hierarchical clustering
		1. ![[dendogram.png]]
3. Principal Component Analysis
	1. Reduce the dimensionality of a data set consisting of a large number of interrelated variables.
	2. Transforming variables into a new set of variables, called the principal components (PCs). PCs are uncorrelated, and are ordered so that the first few retain most of the variation present in all of the original variables


![[Pasted image 20230310173905.png]]
	
	???	DEEP LEARNING
???	Recommender Systems

???	Ensemble Techniques ??? Ada boosting, Gradient Boosting, XG Boosting

???	ROC curve / AUC
???	Strategies for handling imbalanced data (change probability cut-off, over sampling(SMOTE), under sampling)
???	Regression ??? Assumptions related topics (Multicollinearity,  VIF, Assumptions about Errors. Log Transformation on  Xs)
???	Feature Selection with SFS
???	AutoML
???	Data transformation: Log Transformation
???	Pipelines (for techie - implementation)
???	Random forest ??? regression
???	 (???.and exploring algorithms in further details)
![[Pasted image 20230310174114.png]]		

        
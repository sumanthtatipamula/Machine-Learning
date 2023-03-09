----
1. Numpy is a Linear Algebra Library for python, the reason it is so important for Data Science with Python is that almost all of the libraries in the PyData Ecosystem rely on NumPy as one of their main building blocks.
2. Numpy is also incredibly fast, as it has bindings to C libraries.
3.  Numpy arrays essentially come in two flavours : vectors and matrices
4. Vectors are strictly 1-d arrays and matrices are 2-d (Note: A matrix can still have onlt one row or one column).
## Methods
1. np.array - supports multi dimension
    1. np.array([1,2,3]) - for single dimension
    2. np.array([[1,2,3], [4,5,6], [7,8,9]]) - for two dimension
2. np.arange(start, stop, step) - creates single dimension array with provided arguments
3. np.zeros
    1. np.zeros(one_dimen_length) - create 1d array with zeros of specified length
    2. np.zeros((row, column)) - creates 2-d array
    3. np.zeros((.,.,.)) - for multidimentsion
4. np.ones
    1. np.one(one_dimen_length) - create 1d array with 1's of specified length
    2. np.one((row, column)) - create 2-d array
5. np.linspace(start, end, count) - inclusive start and end and returns an 1-d array with equally spaced
6. np.eye(n) - returns an identity matrix of size n * n
7. np.random.rand - values lies between 0 and 1
    1. np.random.rand(size) - returns an 1d array with random values of size
    2. np.random.rand(row, column) - returns an 2d array with random values of size r * c
8. np.random.randn - returns random value from standard normal distribution.
    1. np.random.randn(size) - returns 1d
    2. np.radon.randn(row, column) - returns 2d
9. np.random.randint(start,end, size) - inclusive start exclusive end
    1. np.random.randint(start, end, size) - creates an 1d array with random values within given range
    2. np.random.randint(start, end, (row, column)) - creates an 2d array with random values within given range
10. shape - return shape of numpy array
11. dtype - returns types of value in array
12. min, max - returns min and max value in the array
    1. arr.min()
    2. arr.max()
13. reshape - to reshape the array(for example 1d to 2d)
    1. arr.reshape(5, 5)

## Indexing and Selection
1.  arr  = np.arange(0, 11) - One dimensional
	1. arr[8] returns element at 9th Position or 8th Index
	2. arr[1:] - slice operatior similar to python
	3. arr[0:5] - return elements from 0 to 4 index.
	4. arr[0 : 5] = 10 all the values from 0 to 4th index will be changed to 10
		1. However same thing can't be done with python lists
	5. By default np array slicing don't result in new copy unlike list in python
		1. slice_of_arr = arr[0:6]
		2. slice_of_arr[:] = 99
		3. In both arr and slice_of_arr values from 0 to 5th Index are changed to 99
	6. To get copy of np array
		1. arr.copy()
2.  `arr_2d = np.array([[5,10,15],[20,25,30],[35,40,45]])`
	1. Indexing can be done in 2 ways
		1. just like in python `arr_2d[1][2]
		2.  `arr_2d[1, 2]`
		3.  To get range of elements  `arr_2d[:2, :1]`
3.  Conditions
	1. arr > 1 returns an boolean array with values True if condition is met else false
	2.  arr_2d[arr_2d > 5] return elements in 2d array which meets this condition

## Operations
1.  Array with array
	1. arr = np.arange(0, 11)
		1.  arr + arr -  adds values index wise
		2.  arr *  arr
2.  Array with Scalars
	1.  arr + 100 - adds 100 to each value in arr
	2.  arr ** 2
	3. arr - 100
	4. arr / 100
3.  Universal Array Functions
	1. np. sq


	



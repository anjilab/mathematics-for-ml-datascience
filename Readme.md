# Chapter 1 Week 1:

## Introduction to NumPy
NumPy is main package for python for any kind of scientific computing.(Numerical python)

### NumPy arrays
Array = core data structure in any programming language for organizing data of same type. In core python, we use lists. List takes up more space in the memory & time to process(Research why more space & time) and have limite functions. Hence we use NumPy array.

Due to its extensive built in function,computing takes very less amount of time so performing on large sets of data is convenient.

Array object in NumPy is ndarray meaning n-dimensional array.

# Creating NumPy Arrays

1. np.array([1,2,3,4]) # creates 1 dimensional array.
2. np.arange(4) # Creates an 1-d array from 0 to n-1 where n=4.
   np.arange(3,21,7) # Creates an array beginning from 3 with incremente dby 7 till end point 21 doesnot include 21
3. np.linspace(0,100,5) # Creates 1D array from 0 to 100 with evenly spaced, its return type  is  float. np.linspace(0,100,5, dtype=int) , here 0 = starting number, final number = 100, number of elements in the evenly spaced array = 5 
4. np.ones(4) # Returns an array filled with 1. float type with length of 4.
5. np.zeros(5) # Returns an array filled with 0. float type with length of 5.
6. np.empty(4) # Returns an array of size 4.
7. np.random.rand() # Returns random number between 0 and 1. 

## To find type of arrays
1. number_type = np.array([1,2,3,4,5]) # number_type.dtype => prints its type
2. string_type = np.array(['anjila']) # string_type => prints its type as ```<U6```, this means 6 length character. i.e unicode string with 6 character length.

### To create multi dimensional array
1. two_d_array = [[1,2,3], [7,8,9]]
2. By reshaping 1-D array into 2D array.
one_dimensional_arr = [1,2,3,4,5,6]
 np.reshape(one_dimensional_arr, (2,3))  # Two rows and three columns.

## To find dimensions & shape
1. two_d_array.ndim # prints 2
2. two_d_array.shape # row * column
3. two_d_array.size # total number of elements

### Array operation
Numpy array can be added,subtracted & multiplied
array_1 = np.array([1,2,3])
array_2 = np.array([4,5,6])
array_1 + array_2
array_1 - array_2
array_1 * array_2

# Broadcasting

While converting one units to another units like m to  km, l to ml and so on, we multiply array with scalar units. For eg:
array_1 = np.array([1,2])
array_1 * 2 # it is mulitplying array with single number. Such concept which allows to perform mathematical operations on arrays of different shapes.


# Slicing 
Slicing allows you to get sub elements or specific elements list from the array. It needs start & end values,begins from start, includes start but do not include end value. eg:array[start:end:step]
[1,24,45,78,99][1:3:2]

# Stacking
feature of numpy for customization of numpy arrays. to join two or more arrays either horizontally or vertically, done along a new axis.


np.hstack((array1,array2))
np.hsplit((array1, how_many_array))
np.vstack((array1,array2))


## Week 1 Lab 2  Solving linear equations

-x1 + 3x2 = 7 & 3x1 + 2x2 = 1 are two linear equations. 
Linear system is said to be consistent if it has no solution and said to be consistent if it has more than one or infinite number of solutions.

We can solve linear equation using matrices and np.linalg.solve(a,b) where a = np.array([
        [-1, 3],
        [3, 2]
    ], dtype=np.dtype(float))

b = np.array([7, 1], dtype=np.dtype(float))

To find determinant of matrix: 
determinant= np.linalg.det(a)


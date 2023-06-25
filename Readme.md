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
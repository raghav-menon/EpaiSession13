## Yield Statement Python

Yield is a keyword in Python that is used to return from a function without destroying the states of its local variable
and when the function is called, the execution starts from the last yield statement. Any function that contains a yield 
keyword is termed a generator. Hence, yield is what makes a generator. The yield keyword in Python is less known off but
has a greater utility which one can think of.

## Assignment

Read the file 'nyc_parking_tickets_extract-1.csv'

### Goal 1
Create a lazy iterator that will return a named tuple of the data in each row. The data types should be appropriate - i.e. 
if the column is a date, you should be storing dates in the named tuple, if the field is an integer, then it should be stored as an integer, etc.

### Goal 2
Calculate the number of violations by car make.

### Note:
Try to use lazy evaluation as much as possible - it may not always be possible though! That's OK, as long as it's kept to a minimum.
-No Test Cases
-Submit pending assignments

## cast
 Function to cast the value to the appropriate datatype

## cast_row
Function which takes one row and sends the elements one by one for casting. Returns a list of casted elements 

## read_violations
An iterator function (the function becomes an iterator because of the yield in the function) which reads lazily (line by line 
from the file) and calls the function for casting. Once the elements are casted to proper datatypes, it is assigned to a named
tuple. Thus this is a lazy iterator returning a namedtuple with the elements of the namedtuple casted to appropriate datatype.

## count_violations
Function to count the violations. Uses a dictionary to count the number of violations by each brand car. If the name of the car is 
blank or the violation description is blank, it is not counted

## count_violations1
Function to count the violations. Uses a dictionary to count the number of violations by each brand car. This would include data 
even if the name of the car is black or violation description is blank

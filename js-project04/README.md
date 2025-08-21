# Day 4 Challenge: Array Cardio Day 1

## Overview
Practice and master essential JavaScript array methods through a series of exercises using real historical data. This challenge focuses on filtering, mapping, sorting, and reducing arrays to extract meaningful information.

## How it Works
- Work with two arrays: one containing inventor objects and another with people's names
- Complete eight exercises that demonstrate different array manipulation techniques
- Use console.table() for better visualization of object arrays
- Implement solutions using various array methods

## Key Concepts Learned
### Array.prototype.filter()
- Creates a new array with elements that pass a test implemented by the provided function
- Example: Filter inventors born in the 1500s by checking year property

### Array.prototype.map()
- Creates a new array with the results of calling a provided function on every element
- Example: Transform inventor objects into strings containing first and last names

### Array.prototype.sort()
- Sorts the elements of an array in place and returns the sorted array
- Can use comparison functions to define custom sort orders
- Example: Sort inventors from oldest to youngest based on birth year

### Array.prototype.reduce()
- Executes a reducer function on each element of the array, resulting in a single output value
- Powerful for transforming arrays into different data structures or calculating aggregates
- Example: Calculate total years lived by all inventors

### Ternary Operator
- Concise alternative to if-else statements for simple conditional logic
- Example: `condition ? exprIfTrue : exprIfFalse`

### Array Destructuring
- Extract multiple properties from array elements in a single statement
- Example: `const [aLast, aFirst] = lastOne.split(", ")`

### Object Property Assignment
- Dynamically create and update properties in objects using bracket notation
- Example: `obj[item] = 0` and `obj[item]++` in the transportation counter

## Learning Outcomes
- Mastering essential array methods for data manipulation
- Transforming data between different formats and structures
- Implementing complex sorting logic with custom comparison functions
- Using reduce() for aggregation and data transformation
- Working with real-world data structures and extracting meaningful information
- Writing clean, functional JavaScript code for data processing

# Array cardio 2

> some methods to apply and array

## Array.prototype.some()

The **some()** method of Array instances tests whether at least one element in the array passes the test implemented by the provided function. It returns true if, in the array, it finds an element for which the provided function returns true; otherwise it returns false. It doesn't modify the array.

Parameters
- callbackFn
A function to execute for each element in the array. It should return a truthy value to indicate the element passes the test, and a falsy value otherwise. The function is called with the following arguments:

- element:
The current element being processed in the array.

- index:
The index of the current element being processed in the array.

- array:
The array **some()** was called upon.

- thisArg (Optional):
A value to use as this when executing callbackFn. See iterative methods.

## Array.prototype.every()
The **every()** method of Array instances tests whether all elements in the array pass the test implemented by the provided function. It returns a Boolean value.

Parameters
- callbackFn:
A function to execute for each element in the array. It should return a truthy value to indicate the element passes the test, and a falsy value otherwise. The function is called with the following arguments:

- element:
The current element being processed in the array.

- index:
The index of the current element being processed in the array.

- array:
The array **every()** was called upon.

- thisArg (Optional):
A value to use as this when executing **callbackFn**. See iterative methods.

## Array.prototype.find()
The **find()** method of Array instances returns the first element in the provided array that satisfies the provided testing function. If no values satisfy the testing function, undefined is returned.

If you need the index of the found element in the array, use **findIndex()**.
If you need to find the index of a value, use indexOf(). (It's similar to **findIndex()**, but checks each element for equality with the value instead of using a testing function.)
If you need to find if a value exists in an array, use **includes()**. Again, it checks each element for equality with the value instead of using a testing function.
If you need to find if any element satisfies the provided testing function, use **some()**.
If you need to find all elements that satisfy the provided testing function, use **filter()**.

Parameters

- callbackFn:
A function to execute for each element in the array. It should return a truthy value to indicate a matching element has been found, and a falsy value otherwise. The function is called with the following arguments:

- element:
The current element being processed in the array.

- index:
The index of the current element being processed in the array.

- array:
The array find() was called upon.

- thisArg (Optional):
A value to use as this when executing callbackFn. See iterative methods.

## Array.prototype.findIndex()
The **findIndex()** method of Array instances returns the index of the first element in an array that satisfies the provided testing function. If no elements satisfy the testing function, -1 is returned.

See also the **find()** method, which returns the first element that satisfies the testing function (rather than its index).

Parameters
- callbackFn:
A function to execute for each element in the array. It should return a truthy value to indicate a matching element has been found, and a falsy value otherwise. The function is called with the following arguments:

- element:
The current element being processed in the array.

- index:
The index of the current element being processed in the array.

- array:
The array **findIndex()** was called upon.

- thisArg (Optional):
A value to use as this when executing **callbackFn**. See iterative methods.

## Array.prototype.splice()
The **splice()** method of Array instances changes the contents of an array by removing or replacing existing elements and/or adding new elements in place.

To create a new array with a segment removed and/or replaced without mutating the original array, use **toSpliced()**. To access part of an array without modifying it, see **slice()**.

**Parameters:**

**start:**

Zero-based index at which to start changing the array, converted to an integer.

- Negative index counts back from the end of the array — if -array.length <= start < 0, start + array.length is used.

- If start < -array.length, 0 is used.

- If start >= array.length, no element will be deleted, but the method will behave as an adding function, adding as many elements as provided.

- If start is omitted (and **splice()** is called with no arguments), nothing is deleted. This is different from passing undefined, which is converted to 0.

**deleteCount (Optional)**:

An integer indicating the number of elements in the array to remove from start.

If deleteCount is omitted, or if its value is greater than or equal to the number of elements after the position specified by start, then all the elements from start to the end of the array will be deleted. However, if you wish to pass any itemN parameter, you should pass Infinity as deleteCount to delete all elements after start, because an explicit undefined gets converted to 0.

If deleteCount is 0 or negative, no elements are removed. In this case, you should specify at least one new element (see below).

**item1**, …, **itemN** (Optional):

The elements to add to the array, beginning from start.

If you do not specify any elements, splice() will only remove elements from the array.


## 📝 License

This project is [MIT](./MIT.md) licensed.

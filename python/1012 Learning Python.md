#  1012 PYTHON DATA TYPE LIST

# "PYTHON LIST"

## List
- Lists are used to store multiple items in a single variable.
- Lists are one of 4 built-in data types in Python used to store collections of data, the other 3 are Tuple, Set, and Dictionary, all with different qualities and usage.
- Lists are created using square brackets:

``` python
thislist = ["apple", "banana", "cherry"]
print(thislist)
```
``` python
thislist = ["apple", "banana", "cherry"]
print(thislist[2])
```

## Allow Duplicates
- Since lists are indexed, lists can have items with the same value:
``` python
thislist = ["apple", "banana", "cherry", "apple", "cherry"]
print(thislist[0])
print(thislist[3])
print(thislist[1])
print(thislist)
```

## List Length
- To determine how many items a list has, use the len() function:
``` python
thislist = ["apple", "banana", "pineapple", "cherry"]
print(len(thislist))
``` 
``` python
thislist = ["cars", "bicycle", "bus", "motorcycle"]
print(len(thislist))
```

## List Items - Data Types
- List items can be of any data type:
``` python
list1 = ["apple", "banana", "cherry"]
list2 = [1, 5, 7, 9, 3]
list3 = [True, False, False]
print(list1)
print(list2)
print(list3)
```

- A list can contain different data types:
``` python
list1 = ["abc", 34, True, 40, "male"]
print(list1)
```
``` python
list1 = ["D", "20", "false", "30.2", "heights"]
print(list1)
```
## Type()
- From Python's perspective, lists are defined as objects with the data type 'list':
``` python
mylist = ["apple", "banana", "cherry"]
print(type(mylist))
```
## The list() Constructor
- It is also possible to use the list() constructor when creating a new list.
- Using the list() constructor to make a List:
``` python
thislist = list(("apple", "banana", "cherry")) # note the double round-brackets
print(thislist)
```
``` python
thislist = list(("cars", "bus", "bicycle")) 
print(thislist)
```
# "PYTHON BASIC LIST OPERATOR"
# Python- Access List Items
## Access Items
- List items are indexed and you can access them by referring to the index number:
## Example
- Print the second item of the list:
         
``` python
thislist = ["cars", "motorcycle", "bus"]
print(thislist[1])
```

         
         
      













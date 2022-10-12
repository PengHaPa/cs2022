#  1012 PYTHON DATA TYPE LIST

# "PYTHON LIST"

## List
- Lists are used to store multiple items in a single variable.
- Lists are one of 4 built-in data types in Python used to store collections of data, the other 3 are Tuple, Set, and Dictionary, all with different qualities and usage.
- Lists are created using square brackets:
## Example
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
## Example
``` python
thislist = ["apple", "banana", "cherry", "apple", "cherry"]
print(thislist[0])
print(thislist[3])
print(thislist[1])
print(thislist)
```

## List Length
- To determine how many items a list has, use the len() function:
## Example
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
## Example
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
## Example
``` python
mylist = ["apple", "banana", "cherry"]
print(type(mylist))
```
## The list() Constructor
- It is also possible to use the list() constructor when creating a new list.
- Using the list() constructor to make a List:
## Example
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
## Negative Indexing
- Negative indexing means start from the end
- -1 refers to the last item, -2 refers to the second last item etc.
## Example
- Print the last item of the list:

``` python
thislist = ["pink", "blue", "white"]
print(thislist[-1])
```
## Range of Indexes
- You can specify a range of indexes by specifying where to start and where to end the range.
- When specifying a range, the return value will be a new list with the specified items.
## Example
- Return the third, fourth, and fifth item:         
``` python
thislist = ["Cars", "bicycle", "bus", "motorcycle", "taxi", "train", "airplane"]
print(thislist[2:5])
```     
- This example returns the items from the beginning to, but NOT including, "motorcycle":
``` python
thislist = ["Cars", "bicycle", "bus", "motorcycle", "taxi", "train", "airplane"]
print(thislist[:3])
```
- This example returns the items from "bus" to the end:
``` python
thislist = ["Cars", "bicycle", "bus", "motorcycle", "taxi", "train", "airplane"]
print(thislist[2:])
```
## Range of Negative Indexes
- Specify negative indexes if you want to start the search from the end of the list:
## Example
- This example returns the items from "motorcycle" (-4) to, but NOT including "airplane" (-1):
``` python
thislist = ["Cars", "bicycle", "bus", "motorcycle", "taxi", "train", "airplane"]
print(thislist[-4:-1])
```
## Check if Item Exists
- To determine if a specified item is present in a list use the in keyword:
## Example
- Check if "bus" is present in the list:
``` Python
thislist = ["Cars", "bus", "motorcycle"
if "bus" in thislist
  print(Yes 'bus' is in the transportaion list)
```






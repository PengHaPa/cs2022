#  1012 PYTHON DATA TYPE LIST

# "PYTHON LIST"

## List
- Lists are used to store multiple items in a single variable.
- Lists are one of 4 built-in data types in Python used to store collections of data, the other 3 are Tuple, Set, and Dictionary, all with different qualities and usage.
- Lists are created using square brackets:
### Example
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
### Example
``` python
thislist = ["apple", "banana", "cherry", "apple", "cherry"]
print(thislist[0])
print(thislist[3])
print(thislist[1])
print(thislist)
```

## List Length
- To determine how many items a list has, use the len() function:
### Example
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
### Example
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
### Example
``` python
mylist = ["apple", "banana", "cherry"]
print(type(mylist))
```
## The list() Constructor
- It is also possible to use the list() constructor when creating a new list.
- Using the list() constructor to make a List:
### Example
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
### Example
- Print the second item of the list:
         
``` python
thislist = ["cars", "motorcycle", "bus"]
print(thislist[1])
```
## Negative Indexing
- Negative indexing means start from the end
- -1 refers to the last item, -2 refers to the second last item etc.
### Example
- Print the last item of the list:

``` python
thislist = ["pink", "blue", "white"]
print(thislist[-1])
```
## Range of Indexes
- You can specify a range of indexes by specifying where to start and where to end the range.
- When specifying a range, the return value will be a new list with the specified items.
### Example
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
### Example
- This example returns the items from "motorcycle" (-4) to, but NOT including "airplane" (-1):
``` python
thislist = ["Cars", "bicycle", "bus", "motorcycle", "taxi", "train", "airplane"]
print(thislist[-4:-1])
```
## Check if Item Exists
- To determine if a specified item is present in a list use the in keyword:
### Example
- Check if "bus" is present in the list:
``` Python
thislist = ["Cars", "bus", "motorcycle"]
if "bus" in thislist:
  print("Yes, 'bus' is in the transportaion list")
```
# Python - Change List Items
## Change Item Value
- To change the value of a specific item, refer to the index number:
### Example
- Change the second item:
``` python
thislist = ["cars", "bus", "airplane"]
thislist[1] = "bicycle"
print(thislist)
```
## Change a Range of Item Values
- To change the value of items within a specific range, define a list with the new values, and refer to the range of index numbers where you want to insert the new values:
- If you insert more items than you replace, the new items will be inserted where you specified, and the remaining items will move accordingly:
### Example
- Change the values "bicycle" and "bus" with the values "horse" and "boat":
``` python
thislist = ["Cars", "bicycle", "bus", "motorcycle", "taxi", "train", "airplane"]
thislist[1:3] = ["horse", "boat"]
print(thislist)
```
- Change the second value by replacing it with two new values:
``` python
thislist = ["cars", "bus", "airplane"]
thislist[1:2] = ["boat", "train"]
print(thislist)
```
- Note: The length of the list will change when the number of items inserted does not match the number of items replaced.
- If you insert less items than you replace, the new items will be inserted where you specified, and the remaining items will move accordingly:
``` python
thislist = ["cars", "bus", "airplane"]
thislist[1:3] = ["motorcycle"]
print(thislist)
```
## Insert Items
- To insert a new list item, without replacing any of the existing values, we can use the insert() method.
- The insert() method inserts an item at the specified index:
### Example
- Insert "boat" as the third item: 
```python
thislist = ["cars", "bus", "airplane"]
thislist.insert(2, "boat")
print(thislist)
```
- Note: As a result of the example above, the list will now contain 4 items.
# Python - Add List Items
## Append Items
- To add an item to the end of the list, use the append() method:
### Example
- Using the append() method to append an item:
``` python
thislist = ["cars", "bus", "airplane"]
thislist.append("boat")
print(thislist)
```
## Insert Items
- To insert a list item at a specified index, use the insert() method.
- The insert() method inserts an item at the specified index:
### Example
- Insert an item as the second position:
```python
thislist = ["cars", "bus", "airplane"]
thislist.insert(1, "motorcycle")
print(thislist)
```
## Extend List
- To append elements from another list to the current list, use the extend() method.
### Example
- Add the elements of land to thislist:
```python
thislist = ["motorcycle", "bus", "car"]
land = ["airplane", "boat", "jet"]
thislist.extend(land)
print(thislist)
```
## Add Any Iterable
- The extend() method does not have to append lists, you can add any iterable object (tuples, sets, dictionaries etc.).
### Example
- Add elements of a transpo to a list:
```python
thislist = ["airplane", "boat", "jet"]
transpo = ("train", "cars")
thislist.extend(thistuple)
print(thislist)
```
# Python - Remove List Items
## Remove Specified Item
- The remove() method removes the specified item.
### Example
- Remove "boat".
```python
thislist = ["airplane", "boat", "jet"]
thislist.remove("boat")
print(thislist)
```
## Remove Specified Index
- The pop() method removes the specified index.
### Example
- Remove the second item:
```python 
thislist = ["airplane", "boat", "jet"]
thislist.pop(1)
print(thislist)
```
- If you do not specify the index, the pop() method removes the last item.
```python 
thislist = ["airplane", "boat", "jet"]
thislist.pop()
print(thislist)
```
- The del keyword also removes the specified index:
- Remove the first item:
```python
thislist = ["airplane", "boat", "jet"]
del thislist[0]
print(thislist)
```
- The del keyword can also delete the list completely.
- Delete the entire list:
```python
thislist = ["airplane", "boat", "jet"]
del thislist
```
## Clear the List
- The clear() method empties the list.
- The list still remains, but it has no content.
### Example
- Clear the list content:
```python 
thislist = ["airplane", "boat", "jet"]
thislist.clear()
print(thislist)
```
# Python - Sort Lists
## Sort List Alphanumerically
- List objects have a sort() method that will sort the list alphanumerically, ascending, by default:
### Example
- Sort the list alphabetically:
```python
thislist = ["cars", "bicycle", "bus", "motorcycle", "taxi", "train", "airplane"]
thislist.sort()
print(thislist)
```
- Sort the list numerically:
```python
thislist = [92, 50, 45, 87, 65, 82, 23]
thislist.sort()
print(thislist)
```
## Sort Descending
- To sort descending, use the keyword argument reverse = True:
### Example
- Sort the list descending:
```python
thislist = ["cars", "bicycle", "bus", "motorcycle", "taxi", "train", "airplane"]
thislist.sort(reverse = True)
print(thislist)
```
- Sort the list descending:
```python
thislist = [92, 50, 45, 87, 65, 82, 23]
thislist.sort(reverse = True)
print(thislist)
```
## Customize Sort Function
- You can also customize your own function by using the keyword argument key = function.
- The function will return a number that will be used to sort the list (the lowest number first):
### Example
- Sort the list based on how close the number is to 10:
```python
def myfunc(n):
  return abs(n - 10)

thislist = [100, 50, 65, 82, 23, 20, 13, 9,]
thislist.sort(key = myfunc)
print(thislist)
```
## Case Insensitive Sort
- By default the sort() method is case sensitive, resulting in all capital letters being sorted before lower case letters:
### Example
- Case sensitive sorting can give an unexpected result:
```python
thislist = ["cars", "Bicycle", "bus", "Motorcycle", "Taxi", "Train", "airplane"]
thislist.sort()
print(thislist)
```
- Luckily we can use built-in functions as key functions when sorting a list.
- So if you want a case-insensitive sort function, use str.lower as a key function:
- Perform a case-insensitive sort of the list:
```python
thislist = ["cars", "Bicycle", "bus", "Motorcycle", "Taxi", "Train", "airplane"]
thislist.sort(key = str.lower)
print(thislist)
```
### Reverse Order
- What if you want to reverse the order of a list, regardless of the alphabet?
- The reverse() method reverses the current sorting order of the elements.
### Example
- Reverse the order of the list items:
```python
thislist = ["airplane", "boat", "jet", "train"]
thislist.reverse()
print(thislist)
```
# Python - Copy Lists
## Copy a List
- You cannot copy a list simply by typing list2 = list1, because: list2 will only be a reference to list1, and changes made in list1 will automatically also be made in list2.
- There are ways to make a copy, one way is to use the built-in List method copy().
### Example
- Make a copy of a list with the copy() method:
```python
thislist = C
mylist = thislist.copy()
print(mylist)
```
- Another way to make a copy is to use the built-in method list().
```python 
thislist = ["airplane", "boat", "jet", "train"]
mylist = list(thislist)
print(mylist)
```
# Python - Join Lists
## Join Two Lists
- There are several ways to join, or concatenate, two or more lists in Python.
- One of the easiest ways are by using the + operator.
### Example 
- Join two list:
```python
list1 = ["A", "B", "C", "D"]
list2 = [2, 4, 6, 8, 10]

list3 = list1 + list2
print(list3)
```
- Another way to join two lists is by appending all the items from list2 into list1, one by one:
- Append list2 into list1:
```python
list1 = ["A", "B", "C", "D"]
list2 = [2, 4, 6, 8, 10]

for x in list2:
  list1.append(x)

print(list1)
```
- Or you can use the extend() method, which purpose is to add elements from one list to another list:
- Use the extend() method to add list2 at the end of list1:
```python
list1 = ["A", "B", "C", "D"]
list2 = [2, 4, 6, 8, 10]

list1.extend(list2)
print(list1)****
```


















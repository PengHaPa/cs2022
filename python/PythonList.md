#  1005 PYTHON DATA TYPE LIST

# "PYTHON LIST"

#List
- Lists are used to store multiple items in a single variable.
- Lists are one of 4 built-in data types in Python used to store collections of data, the other 3 are Tuple, Set, and Dictionary, all with different qualities and usage.
- Lists are created using square brackets:

'''python
thislist = ["apple", "banana", "cherry"]
print(thislist)

thislist = ["apple", "banana", "cherry"]
print(thislist[2])

Allow Duplicates
-Since lists are indexed, lists can have items with the same value:

thislist = ["apple", "banana", "cherry", "apple", "cherry"]
print(thislist[0])
print(thislist[3])
print(thislist[1])
print(thislist)

List Length
-To determine how many items a list has, use the len() function:

thislist = ["apple", "banana", "pineapple", "cherry"]
print(len(thislist))

List Items - Data Ty-pes
-List items can be of any data type:

list1 = ["apple", "banana", "cherry"]
list2 = [1, 5, 7, 9, 3]
list3 = [True, False, False]
print(list1)
print(list2)
print(list3)

-A list can contain different data types:

list1 = ["abc", 34, True, 40, "male"]
print(list1)

Type()
-From Python's perspective, lists are defined as objects with the data type 'list':

mylist = ["apple", "banana", "cherry"]
print(type(mylist))

The list() Constructor
-It is also possible to use the list() constructor when creating a new list.
-Using the list() constructor to make a List:

thislist = list(("apple", "banana", "cherry")) # note the double round-brackets
print(thislist)














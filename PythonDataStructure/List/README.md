# Python List

## From Python's Site

1. List operators

* **list.append**

* **list.extend(iterable)**

* **list.insert(position, item)**: Insert an item at a given position.

* **list.remove(x)**: Remove the first item from the list whose value is equal to x

* **list.pop(position)**: Remove the item at the given position in the list. If no index is specified, a.pop() 
removes and return the last item in the list.
> Notice: a.pop() not a.pop it just return the function call

* **list.clear()**: remove all items from the list
> a = [1, 3, 4]
>
> a.clear()
>
> print(a) # return []

* **list.index(x[, start[, end]])**: Return zero-based index in the list of the first item whose value is x. Raise 
ValueError if there is no such item.
Optional argument start and end is slice notation used to limit the search to a subsequence of list. The returned index 
is computed from the begin of the list.

> Example
> a = [1, 2, 3, 4, 5, 6, 7, 8, 9, 5, 6, 7, 2, 4, 5]
>
> a.index(5) # return 4
>
> a.index(5, 5, len(a) - 1) # return 9
>
> a.index(5, 20, 25) # Value error 5 not in the list


* **list.count(x)**: Return number of times x appears in the list
> Example: 
>
> a = [1, 2, 3, 4, 5, 6, 7, 8, 9, 5, 6, 7, 2, 4, 5]
>
>a.count(5) # Return 3
>
>a.count(10) # Return 0
>
>a.count('a') # Return 0
>

* **list.sort(key=None, reverse=False)**: Sort the items in the list in place (mean the list is change). The arguments 
can be used for sort customization. 

More specific about the key argument: 

key specifies a function of one argument that used to extract a comparison key from each element in iterable  (example: 
key=str.lower). Default is none.
 
 
2. List Notation
* Slice notation: 
Full slice syntax is: start:stop:step


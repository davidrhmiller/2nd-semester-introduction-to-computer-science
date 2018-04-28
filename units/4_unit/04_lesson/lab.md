# Lab 4.04 - Shopping List

## Part 1
The goal of this lab is to practice using and accessing items from lists of lists. 

Here's a [scaffold of the program][1] with all the interesting bits left for you to write (we've taken care of the boring bits)

[1]: https://repl.it/@davidrhmiller/TEALS2018-Lab-404-Shopping-List-scaffolding

You have a few errands to run and have created a few shopping list to help you remember what to buy. You stored your notes in a nested list, `shopping_cart`. 
This program will allow the user to ask for a specific item by it's index or update what items are in the cart. The user can request you `print all` the items in a specific shopping list.

###Schedule 

```python
shopping_cart = [
['tooth paste', 'q-tips', 'milk'],
['milk', 'candy', 'apples'],
['planner', 'pencils', 'q-tips']
]
```

### User Inputs
* `update`
	* The program will ask which shopping list the user wants to update, which position it should update, and the new value to update.
* `print` 
	*  The program will ask which shopping list the user wants to print from and afterwards will request which position it should print.
* `print all`
	* The program will ask which shopping list the user wants to print and will print all of the items associated with that shopping list. 	
	
###Functions
* `update_list`
    * Takes in an integer representing the index of the shopping list, an integer representing the index of the item to update, and a string representing the new item to add to that shopping list.
* `print_item`
    * Takes an int representing the index of the shopping list followed by an int representing the index of the item to print.
* `print_list`
    * Takes an int representing the index of the shopping list to print.

* Feel free to add more functions as you see fit

### Example

```
>>>What would you like to do? print all
Which shopping list would you like to print? 1
tooth paste, q-tips, gum
```

## Part 2 

In this part of the lab you will go through your shopping list program and perform a few different calculations. 

1. Create a function, `all_in_one`, that will put all the shopping lists into a single list using a for loop. 
2. Create a function, `count_q_tips`, which will go through all items of the list and keep a count of how many times `'q_tips'` occurs. 
3. In order to make the shopping lists more calcium rich, write a function, `drink_more_milk`, that adds `'milk'` to each of the lists (unless it's already there). 
4. You can't have milk without cookies. Write a function `if_you_give_a_moose_a_cookie`, that will go through every element of schedule and update `'milk'` to be `'milk and cookies'`.

###Bonus! 
Write a function to reverse the order of the lists and items in `shopping_cart`. 

The list should look like the following when printed: 

```python
schedule = [
['q-tips', 'pencils', 'planner'],
['apples', 'candy', 'milk'],
['milk', 'q-tips', 'toothe paste']
]
```

###Tip
Last item can be gotten by `my_list[-1]`

Second to last element: `my_list[-2]`

Third to last element: `my_list[-3]`

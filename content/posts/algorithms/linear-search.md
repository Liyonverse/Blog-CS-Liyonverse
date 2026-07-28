---
title: "Algorithms"
date: 2026-07-28
author: Liyonverse
tags: [Algorithms, Computer Science]
cover : "algo.jpg"
---

# Linear search

---

# What is this algorithm?

<!--more-->

> **Difficulty:** Intermediate 

> **Estimated Reading Time:** 10 minutes




Linear search is one of the simplest algorithms in computer science. It works by looking at each element in a list, one by one, to find a target value.

How it works:

- It checks the first element in the list.

- If it finds the target value, it stops and returns that element (or its index position).

- If it doesn't match, it moves to the next element and checks again.

- It keeps doing this until it finds the target or reaches the end of the list.

You can run a linear search from left to right or from right to left—it checks items in a straight line either way

---

# Simple Example to understand this

Real-Life Example: Finding Your Locker

Imagine you are standing in front of a row of 7 lockers, and each locker has a name tagged on it. You are trying to find the locker with your name on it.

Here is how you would do it:

- Start at the beginning: Go to the very first locker.

- Check the name: Look at the tag.

- If it has your name, congratulations! You found it, and your search is finished.

- If it has someone else's name, move to the next locker.

- Repeat: Keep checking the lockers one by one (Locker 2, Locker 3, and so on).

- Finish: You stop as soon as you find your name, or after you check all 7 lockers.

That is exactly how Linear Search works! It checks items one by one in a straight line until it finds what it's looking for.

---

# Why do we need it?

You might wonder why we need linear search if there are faster algorithms available. Here is why it is so useful:

- Works on unsorted data: Linear search doesn't require your data to be in order. If your list is mixed up, linear search still works!

- Great for small datasets: If you only have a few items (like 10 or 20), linear search is fast enough and requires zero preparation.

- Super easy for beginners: It is the simplest search concept to code and understand.

- The foundation for harder algorithms: Learning linear search first makes it much easier to understand more advanced algorithms, like Binary Search.

Pro Tip for Beginners: Before jumping straight into Binary Search, I highly suggest coding a Linear Search first. It helps build your problem-solving confidence!

---

# Real-World Applications

Where is this algorithm used?

📱 Contact List

Searching a name in a small contact list.

🎵 Music Playlist

Finding a specific song in your playlist.

📚 Library

Searching for a book in a small collection.

🛒 Shopping List

Checking whether an item exists.

🎓 Student Attendance

Finding whether a student's name is present.

🎮 Games

Searching for a player or item in a small inventory.

📝 To-Do Apps

Finding a specific task.

---

# Prerequisites

Before learning this algorithm, you should know:

- Variables
- Lists/Arrays
- Loops (for or while)
- If statements
- Comparison operators (==, <, >)

Now that you understand how these things works, the best way to solidify your learning is to write the algorithm yourself!

---


# Example

Input

```
array [ 20 , 34 , 12 , 50 ]
I need number "12"
```

Process

- Go to fist number
- if the number is "12". finish search and say "Victory!" .else,
- go to next number.
- if the number is "12". finish search and say "Victory!" .
- else do 3rd Line

Output

```
number "12" and Victory!
```

---


# Python Implementation

```python
# mylist = [ 24 , 12 , 30 , 45 , 3 ]

mytarget = 30

count = 0
while (count<len(mylist)):
    if mylist[count] == mytarget:
        print("found at index",count)
        break
    else:
        count += 1 
```

# What's hapenning ?

- mylist and mytarget: We have a list of numbers, and we are looking for the number 30.

- count = 0: We start at index position 0 (the very first item, which is 24).

- while (count < len(mylist)): This tells Python, "Keep looping through the list until you reach the end."

- if mylist[count] == mytarget: Python checks, "Is the current item equal to 30?"

- If YES: It prints where it found it and runs break to instantly stop searching.

- If NO: It goes to else, adds 1 to count (count += 1), and checks the next item in the next loop.

What happens inside each loop?
- Loop 1 (count = 0): Checks 24. Is 24 == 30? No! Moves to next (count = 1).

- Loop 2 (count = 1): Checks 12. Is 12 == 30? No! Moves to next (count = 2).

- Loop 3 (count = 2): Checks 30. Is 30 == 30? Yes!

Result: Prints "found at index 2" and stops completely

# Time Complexity

| Case | Complexity |
|------|------------|
| Best |  O(1)      |
| Worst |  O(n)     |

---

# Advantages

- ✔Easy to understand: It is simple, logical, and great for beginners who are just starting to learn programming.

- ✔Works on any dataset: It doesn't matter if your list is sorted or unsorted—linear search will still find your target item.

- ✔Perfect for small lists: For short lists with just a few items, linear search is fast, simple, and gets the job done without extra setup.

- ✔No extra memory needed: It searches the list directly in place, so it doesn't waste computer memory.


---

# Disadvantages

- ✘Gets slow on large datasets: As the size of your list grows, the time it takes to search increases. If you have 1,000,000 items, it might have to check all         1,000,000 items in the worst case!

- ✘Less efficient than other algorithms: Compared to faster algorithms like Binary Search, linear search is much slower on big lists.



---

# Summary

What it is: Linear search is a simple algorithm that checks items in a list one by one until it finds the target.

When to use it: It is best for small lists or unsorted data.

Pros: Super easy to understand and code.

Cons: Gets very slow as your list gets larger.

Next Step: Once you feel comfortable writing Linear Search, you are ready to learn Binary Search!
---


# References

- Harward university
- Open AI

---

⭐ Thanks for reading!

If you found this helpful, feel free to star the repository and follow my learning journey...

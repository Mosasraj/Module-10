# Queue-Remove Two String Values from the Rear End in Python 🧵

This Python program demonstrates how to manage a list of strings and remove the last two elements (i.e., from the rear of the list).

## 🎯 Aim

To write a Python program to:
- Accept `n` string values from the user
- Remove the last two values (rear end of the list)
- Display the updated list

## 🧠 Algorithm

1. Create an empty list `q`.
2. Read an integer `n` from the user (number of strings).
3. Loop `n` times:
   - Read a string input.
   - Append it to the list `q`.
4. Remove the last element using `pop()`.
5. Remove the next last element using `pop()` again.
6. Display the updated list.

##  Program:
```
queue = []
n = int(input("Enter the number of elements in the queue: "))
for i in range(n):
    value = int(input(f"Enter element {i + 1}: "))
    queue.append(value)
if len(queue) >= 2:
    queue.pop(0)
    queue.pop(0)
elif len(queue) == 1:
    queue.pop(0)
    print("Only one element was in the queue, so it's now empty.")
else:
    print("The queue is empty. Nothing to remove.")
if queue:
    queue.sort(reverse=True)
    print("Remaining elements in descending order:", queue)
else:
    print("No elements remaining in the queue.")
```

### Output:
![image](https://github.com/user-attachments/assets/1bddd868-2dae-49c6-8a4b-cc59391e361d)

## Result:
```
Thus the program has been executed successfully.
```

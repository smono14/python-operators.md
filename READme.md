🔍 Python Tips: Understanding the Difference Between is and in
If you're working with Python, you've likely come across the operators is and in — and while they look similar, they serve very different purposes.

Let’s break it down with examples and key concepts 🧵👇

✅ is — Identity Operator
is checks whether two variables point to the same object in memory (i.e., identity), not whether their values are equal.

📌 Example:

python
Copy
Edit
a = [1, 2, 3]
b = a
c = [1, 2, 3]

print(a is b)  # True — same memory reference
print(a is c)  # False — same values, different objects
print(a == c)  # True — values are equal
✅ in — Membership Operator
in checks whether an element exists inside an iterable (like a list, tuple, set, or string).

📌 Example:

python
Copy
Edit
colors = ['red', 'green', 'blue']

print('green' in colors)  # True
print('yellow' in colors) # False
Also works with strings:

python
Copy
Edit
'Py' in 'Python'  # True
'x' in 'Python'   # False

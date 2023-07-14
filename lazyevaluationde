This example illustrates lazy evaluation using generators in Python:

```python
# Generator function for an infinite sequence of even numbers
def even_numbers():
    number = 0
    while True:
        yield number
        number += 2

# Lazy evaluation example
even_nums = even_numbers()

# Take the first five even numbers
first_five = [next(even_nums) for _ in range(5)]

# Print the first five even numbers
print(first_five)  # Output: [0, 2, 4, 6, 8]

# Continue the sequence, but only until the first even number greater than 10
next_even = next(n for n in even_nums if n > 10)

# Print the next even number greater than 10
print(next_even)  # Output: 12
```
"""
In this example, we define a generator function `even_numbers()` that generates an infinite sequence of even numbers. Instead of generating the entire sequence upfront, the generator produces numbers on-demand, following a lazy evaluation strategy.

We demonstrate lazy evaluation by first taking the first five even numbers from the `even_nums` generator using a list comprehension. Only the necessary elements are computed and stored in the `first_five` list.

Next, we continue the sequence by finding the next even number greater than 10 using a generator expression combined with the `next()` function. The generator expression evaluates the sequence lazily, stopping as soon as it finds the desired condition.

Lazy evaluation allows us to work with potentially infinite or large sequences without the need to compute or store all elements at once. It optimizes memory usage and improves performance by deferring computation until it is required.

Note: In Python, certain functions and operations, such as `range()` and slicing of lists, also exhibit lazy evaluation characteristics, returning generators or iterators instead of creating the entire sequence upfront.
"""

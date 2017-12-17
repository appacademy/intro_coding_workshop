## Learning Goals

1. Understand the use cases for arrays
2. Become familiar with the most widely used array methods

---

### Arrays

Arrays store sequences of objects, separated by commas.
Why is that useful? Well, this **_data structure_** provides us a
handy way to store lists of values that are related in a single variable.

```ruby
cool_things = ["Racecars", "Lasers", "Aeroplanes"]
four_primes = [2, 3, 5, 7]
an_empty_array = []
```

---

### Indexing

Arrays wouldn't be very useful if we couldn't get things out of them.
So how are we going to access a specific value within the array?

The answer: indices.

Think of an index as the position of a value in the list. Indices ALWAYS
start at 0 in programming. So if you want the first value in the list
(reading from left to right), you'll access the O<sup>th</sup>
position. The second value from the first and so on.

You can also change a specific position's value, so in that way, an array
is very much like a group of ordered variables.

Note:

Tell them it's normal to think that's odd. Maybe tell them why that's the
case. Reassure them it'll come naturally with practice.

```ruby
cool_things = ["Racecars", "Lasers", "Aeroplanes"]

puts(cool_things[0])
puts(cool_things[1])
puts(cool_things[2])

cool_things[2] = "Airplanes"
puts cool_things[2]
```

---

### Push + Pop

Although indexing into an array allows us to access and manipulate an
element in a specific position of the array, we often need to just add
or remove from the end of the array.

```ruby
favorite_animals = []

favorite_animals.push("dog")

puts favorite_animals

favorite_animals.push("cat")

puts favorite_animals

favorite_animals.pop

puts favorite_animals
```

---

### Unshift + Shift

These two functions are the same as push and pop, respectively, but
will add or remove from the beginning of the array. Let's take a moment
to try this out again in the REPL environment.

---

### Looping through Array

```ruby
# You can write an array across many lines like this.
presidents = [
  "George Washington",
  "John Adams",
  "Thomas Jefferson",
  "James Madison",
  "James Monroe",
  "John Quincy Adams"
]

# Prints 6, the number of items in the array
puts(presidents.length)

# Print each one of the presidents in the array.
idx = 0
while idx < presidents.length
  puts(presidents[idx])
  idx = idx + 1
end

puts("PRESIDENTS LOOP COMPLETED!")
```

Note:
point out the array length method as intro to methods on data structures
this is a common use case for using arrays (iterating through lists)

---

### CODE

1. Write a program that creates an array and prints a list of cities
you have lived in. Keep in mind `puts array` will print the list element
by element.

2. You are given the array `[nil,nil,nil,nil,nil]`. Write a program that
loops through the array (from beginning to end) and prints the phrase
"I love App Academy" every time. You should see the phrase five times.

3. You are given the array [1,2,3,4,5]. You are asked to loop through the array and replace each position with the product of the number at that position and the index. Print out the new array.

---

## Review

+ Array Indexing
+ Push / Pop
+ Unshift / Shift
+ Looping through an Array

---

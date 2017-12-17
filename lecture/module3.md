## Learning Goals

1. Become familiar with the `while` loop
2. Practice effectively using logical operations as a looping condition

---

### `while` loops

```ruby
condition = true
i = 0

while condition
  puts "This code will execute until the condition is false"
  if i == 3
    condition = false
  end
  i += 1 # incrementing variable
end
```

Note:

Go through the anatomy of this while loops

---

### Looping with User Input

```ruby
puts("Input a number!")
num = gets.to_i

while num < 100
  puts("That number is too small! Try again!")
  # prompt again, re-assign `num`
  num = gets.to_i
end

puts("You typed " + num.to_s + " which is at least 100!")
```

---

### CODE

1. Write a loop that prints out the numbers 1 - 9.

2. Let's go back to the first example. Write a loop that prints out
the statement "Hello, World!" three times with as least code as possible.

3. Given a specific number, write a program that will print `true` if the
number is prime and `false` if the number is not.

Note:

Give them the algorithm to determine if a number is prime so they just
need to code it out

---

### Infinite Loops

```ruby
puts "Print statements forever"
while true
  puts "and ever"
end
```

---

## Review

1. Finite + Infinite looping using `while`
1. Incrementing / Decrementing Variable
2. Logical Operations in Conditions

---

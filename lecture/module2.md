## Learning Goals

1. Become familiar with a if ... elsif ... else statements
1. Practice effectively using logical operations as conditions

---

### Conditional Statements

Keep in mind - although what we've covered seems very mathematically
oriented, programming is really just supposed to be a way to tell
a computer what you would do as a person.

For that reason, we need to discover the tools that are available to us
for us to continue problem solving.

---

### If ... Else

```ruby
condition = true
if (condition)
  puts "You will never know my secrets"
else
  puts "Deepest Darkest Secret: I love Corgis"
end
```

Note:

Talk about the syntax here. Note what has conditions and notice the
single `end` statement. They most likely haven't been exposed to `end`
until now, so go over what that means.
`else` also happens at the very last bit

This is an example of control flow

TODO: add a bit about the phrase `control flow`

---

In English, we naturally have conditional logic. Check out the following
scenario:

"If it's past my bedtime, I'll tell my parents I'm going to sleep. If I
have one hour left, I'll tell them I'm going to watch a show. Otherwise,
I'm going to just tell them I love them."

---

```ruby
if (time > bedtime)
  # notice that this code is indented - that can be done using a single
  # tab
  puts "Parents, I'm going to sleep"
elsif (time == bedtime - 1)
  puts "Parents, I'm going to watch a show"
else
  puts "Parents, I love you"
end
```

Note:

Make sure to explain the syntax for commenting in Ruby. Also note
that there are multiple ways to do comments (multi-line comments) and
that they differ from language to language.

---

### CODE

1. Write a series of conditional statements that will print the statement
"this number is even" if a given number is even, print the statement
"this number is odd" if a given number is odd, and print "this number is
neither even or odd" for all other situations.

2. Write a series of conditional statements that will print the
string "fizz" if the given number is divisible by 3 or the string
"buzz" if the given number is divisible by 5. Otherwise print the number.

---

### AND

```ruby
puts("Input a number!")

number = gets.to_i
if (number > 10) && (number < 20)
  puts("Your number was greater than ten AND less than twenty!")
else
  puts("Your number was either less than ten, OR greater than twenty!")
end
```

Note:

This is the first time we ask for user input. Take a moment to talk about
the `gets` method
I find it useful to think of `gets` and `puts` as opposites

---

### OR

```ruby
puts("Input a number!")

number = gets.to_i
if (number == 7) || (number == 13)
  puts("Your number is magic!")
else
  puts("Your number is not magical")
end
```

---

### Common Mistake

```ruby
# Wrong!
puts("Input a number!")

number = gets.to_i
if number == (7 || 13) # MISTAKE
  puts("You input a magic number!")
else
  puts("Your number is not magical")
end
```

---

### CODE

1. Let's extend the `Fizzbuzz` problem we encountered earlier.
Write a series of conditional statements that will print the
string "fizz" if the given number is divisible by 3, the string
"buzz" if the given number is divisible by 5, or the string "fizzbuzz"
if the number is divisible by both 3 and 5. Otherwise print the number.

2. Write a series of conditional statements that print "found" if the given
number is between the numbers 1 - 10 or is 25. Otherwise, print
"definitely not found"

---

## Review

1. Logical Operations in Conditions
2. Conditional Statements
  + `if`
  + `elsif`
  + `else`

---

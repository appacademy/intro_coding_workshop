# Introduction to Coding Workshop

---

# Hi, I'm Kelly

Note: short blurb about myself

---

### Lecture Agenda

1. Shameless Plug
2. Getting Started
3. Fundamental Programming Concepts
  + Numbers
  + Data Types
  + Variables
  + Methods
  + Logic and Control Flow
  + Data Structures - Arrays + Strings
4. Personal Computer Configuration

---

## App Academy

App Academy is the leading coding bootcamp that only costs money if you find a job (which happens over 95% of the time). In 12 fast paced weeks you'll go from minimal (or none) programming knowledge to being a full-stack web developer, with interviews at the top companies in the country.

---

### What is Programming?

When you write a computer program, you are telling your computer how to do something. As a programmer, your job is to take a larger task and break it down into smaller tasks. You then break down these smaller tasks further until you get to the simplest, most basic tasks that the computer already understands.

The first language you'll be learning at App Academy is **Ruby**

---

### Why Ruby?

Ruby is an elegant programming language perfect for anyone who is beginning to code. It is also powerful and expressive, which makes it a great choice for advanced programmers.

---

### Getting Started

1. Open `https://repl.it/`
2. Please search for and choose the language `Ruby`
3. Type in `puts "Hello, World!"` + click `run`

Note:

Talk to them about what `puts` does
Make sure to note that printing out words require quotation marks around the word
Mention that words are known as `strings` and letters are known as `chars`
---

### Congratulations, you just ran your first program

![congratulations](https://media.giphy.com/media/fxsqOYnIMEefC/giphy.gif)

---

### R-E-P-L

+ Read - Evaluate - Print - Loop
+ Interactive computer programming environment that takes single user inputs (i.e. single expressions), evaluates them, and returns the result to the user

Note:

"Now that we have an environment we can all work in, let's get down to the basics"

---

### Coding Basics

---

### Numbers

+ Integers vs Floats
  * 1 vs 1.0
+ No commas in long integers!
+ `+`, `-`, `*`, `/`, `%`
  * `/`: rounds down
  * `%`: modulo operation => remainder
+ Order of Operations still applies!

---

### Number Practice

```ruby
puts 2 + 5
puts 2 - 5
puts 2 * 5
puts 2 / 5
puts 2.0 / 5.0
puts 2 % 5
puts (2+5) * 6 / 3
```

---

### More Division + Modulo Practice

```ruby
25 / 4
1 / 17
0 / 17

24 % 5
1 % 4
0 % 8
```

---

### Data Types

+ Numbers
  * integers, floats
+ Strings
  * letters, words, characters
+ Boolean
  * `true`, `false`
+ Nil
  * a word to describe absence of data or emptiness

---

### Data Conversion / Coercion

+ `to_i` => to integer
+ `to_s`=> to string

```ruby
puts "5" + "5"
puts "5".to_i + "5".to_i
puts (5 + 5).to_s
puts 5.to_s + 5.to_s
puts "5" + 5
puts "5" * 5
```

---

### Before Variables

Let's say we want to print out `Hello, World!` three times.

```ruby
puts "Hello, World!"
puts "Hello, World!"
puts "Hello, World!"
```

---

### After Variables

Let's shorten the amount of code, by storing the string in variable

```ruby
phrase = "Hello, World!"
puts phrase
puts phrase
puts phrase
```

---

### Variables

+ A variable name consists of letters and numbers
+ The first character needs to be a (lowercase) letter
+ Variables must not contain spaces.
+ When the name of a variable consists of multiple words, it is Ruby convention to separate the words with a `_`
+ The value assigned to the variable can change over time
+ `=` is the assignment operator => you can use it to assign or re-assign values to variables

---

### Methods

+ Methods are the "verbs" of Ruby. Numbers and strings are the objects or "nouns"
+ When you `call` or `invoke` a method, it does something to one or more objects
+ When we call a method, we always use the format `object.method`
  + To the left of the dot is the noun, to the right of the dot is the verb

```ruby
"7".to_i
42.to_s
```

---

### Methods So Far

+ `+`
+ `-`
+ `*`
+ `/`
+ `%`
+ `puts`
+ `to_i`
+ `to_s`

---

### Comparison Methods

+ `<`
+ `>`
+ `!`
+ `==`
+ `!=`

Note:

Mention common mistake between `=` and `==`

---

```ruby
puts 2 < 5
puts 2 > 5
puts 2 == 5
puts 2 != 5
puts 5 == "5"
puts "a" < "b"
puts !true
puts !false
```

---

### Conditional Statements

Keep in mind - although what we've covered seems very mathematically
oriented, programming is really just supposed to be a way to tell
a computer what you would do as a person.

For that reason, we need to discover the tools that are available to us
for us to continue problem solving.

In English, we naturally have conditional logic. Check out the following
scenario:

"If it's past my bedtime, I'll tell my parents I'm going to sleep. If I
have one hour left, I'll tell them I'm going to watch a show. Otherwise,
I'm going to just tell them I love them."

---

### If ... Else

```ruby
if (true)
  puts "You will never know my secrets"
else
  puts "Deepest Darkest Secret"
end
```
Note:

Talk about the syntax here. Note what has conditions and notice the
single `end` statement. They most likely haven't been exposed to `end`
until now, so go over what that means.
`else` also happens at the very last bit

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

### Mistake

```ruby
# Wrong!
puts("Input a number!")

number = gets.to_i
if number == (7 || 13)
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

### Looping

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

1. Let's go back to the first example. Write a loop that prints out
the statement "Hello, World!" three times with as least code as possible.

2. Given a specific number, write a loop that will print `true` if the
number is prime and `false` if the number is not.

---

### Infinite Loops

Note: Demo an infinite loop

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

1. You are given the array `[nil,nil,nil,nil,nil]`. Write a program that
loops through the array (from beginning to end) and prints the phrase
"I love App Academy" every time. You should see the phrase five times.

2. You are given the array `[1,2,3,4,5,6,7,8,9]`. Write a program that
loops through the array and prints the number of values that are prime.

---

### Strings

Similar to arrays, but specifically a data type for words

```ruby
my_string = "Hello World!"
puts(my_string.length) # prints 12

i = 0
while i < my_string.length
  # prints out the letters of "Hello World" one-by-one, each on its own
  # line.
  puts(my_string[i])

  i = i + 1
end
```

---

### String Split

```ruby
"I am a sentence!".split == ["I", "am", "a", "sentence!"]
"word".split("") == ["w", "o", "r", "d"]
```

---

### Code

Write a loop that goes through each character of a string a prints the
number of vowels in the word.

---

Let's say we want to be able to loop 3 times to print any phrase we want.
The code would look something like this.

```ruby
i = 0
while (i < 3)
  puts word
  i += 1
end
```

But the issue is, the variable `word` has to be defined before the loop
starts. What if we want to just tell the program to print any word.

---

### Function

+ A function is a block of organized, reusable code that is used to
perform a single, related action
+ they can have inputs (aka arguments) and outputs

```
f(x) = 2x + 5
```

Note:

Go over what would be considered the input + output

---

### Anatomy of a Method / Function

```ruby
def print_word(word) # def, name of method, arguments for method
  while (i < 3)
    puts word
    i += 1
  end
end
```

Note:

Tell them in Ruby, methods + functions are interchangeable terms

---

### Return Statement

+ The value that follows the `return` is the output of a function
+ Not all functions need to return something, but typically do

```ruby
def count_vowels(word)
  vowels = ["a", "e", "i", "o", "u"]
  num_vowels = 0
  word.split("").each do |character|
    if vowels.include?(character)
      num_vowels += 1
    end
  end

  return num_vowels
end
```

Note:

go over what the return statement does and implicit returns

---

### CODE

1. Write a method that will take a string as input, and return a new
string with the same letters in reverse order.

2. Write a method that takes an integer `n` in; it should return
`n*(n-1)*(n-2)*...*2*1`. Assume n >= 0. As a special case,
`factorial(0) == 1`.

3. Write a method that takes in a string. Return the longest word in
the string. You may assume that the string contains only letters and
spaces.

4. Write a method that takes in an integer `num` and returns the sum of
all integers between zero and num, up to and including `num`.

5. Write a method that takes a string and returns true if it is a
palindrome. A palindrome is a string that is the same whether written
backward or forward. Assume that there are no spaces; only lowercase
letters will be given.

Note:
these will be problems they'll practice after installing the dotfiles

---

### Atom and Dotfiles

Note:

https://github.com/appacademy/dotfiles
Since they won't have access to the dotfiles, we probably need to pull
them into a public repo temporarily.

Maybe even publicize the repo.

---

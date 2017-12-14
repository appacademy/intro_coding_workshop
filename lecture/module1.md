## Learning Goals

1. Become familiar with a REPL environment
2. Learn about the fundamentals of programming
  + Numbers + Basic Mathematic Operations
  + Data Types
  + Variables
  + Methods
  + Logical Operations

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
puts 25 / 4
puts 1 / 17
puts 0 / 17

puts 24 % 5
puts 1 % 4
puts 0 % 8
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

### Comparison Operations

+ `<`
+ `>`
+ `!`
+ `==`
+ `!=`

Note:

Mention common mistake between `=` and `==`

---

### REPL IT

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

Note:

They will do that in their own REPL environments for slides with this title

---

## Review

+ REPL
+ `+`, `-`, `*`, `/`, `%`
+ Data Types
+ Variables and Methods
+ `<`, `>`, `!`, `==`, `!=`

---

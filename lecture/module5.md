## Learning Goals

1. Understand what a function / method is
2. Learn how to define a method with and without a return value

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

1. Define a method that takes two integer values as arguments and returns
the sum of the values.

2. Define a method that takes an array of integer values and returns
the sum of those integer values.

---

## Review

+ What a method is
+ Anatomy of a method
+ `return` statement

---

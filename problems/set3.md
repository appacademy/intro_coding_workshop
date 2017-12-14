## Problem Set 3

1. Write a method that takes in two numbers. Return the greatest
integer that evenly divides both numbers. You may wish to use the
`%` modulo operation.

```ruby
puts("\nTests for #greatest_commmon_factor")
puts("===============================================")
    puts(
      'greatest_common_factor(3, 9) == 3: ' +
      (greatest_common_factor(3, 9) == 3).to_s
    )
    puts(
      'greatest_common_factor(16, 24) == 8: ' +
      (greatest_common_factor(16, 24) == 8).to_s
    )
    puts(
      'greatest_common_factor(3, 5) == 1: ' +
      (greatest_common_factor(3, 5) == 1).to_s
    )
puts("===============================================")
```

2. Write a method that takes in an integer `offset` and a string.
Produce a new string, where each letter is shifted by `offset`. You
may assume that the string contains only lowercase letters and
spaces.

When shifting "z" by three letters, wrap around to the front of the
alphabet to produce the letter "c".

You'll want to use String's `ord` method and Integer's `chr` method.
`ord` converts a letter to an ASCII number code. `chr` converts an
ASCII number code to a letter.

You may look at the ASCII printable characters chart:

    http://en.wikipedia.org/wiki/ASCII#ASCII_printable_characters

Notice that the letter 'a' has code 97, 'b' has code 98, etc., up to
'z' having code 122.

You may also want to use the `%` modulo operation to handle wrapping
of "z" to the front of the alphabet.

```ruby
puts("\nTests for #caesar_cipher")
puts("===============================================")
    puts(
      'caesar_cipher(3, "abc") == "def": ' +
      (caesar_cipher(3, 'abc') == 'def').to_s
    )
    puts(
      'caesar_cipher(3, "abc xyz") == "def abc": ' +
      (caesar_cipher(3, 'abc xyz') == 'def abc').to_s
    )
puts("===============================================")
```

## Problem Set 1

1. Write a method that will take an array of letters as input, and
return a new array of letters with the same letters in reverse order.

```ruby
puts("\nTests for #reverse")
puts("===============================================")
    puts(
      'reverse("abc") == "cba": ' + (reverse("abc") == "cba").to_s
    )
    puts(
      'reverse("a") == "a": ' + (reverse("a") == "a").to_s
    )
    puts(
      'reverse("") == "": ' + (reverse("") == "").to_s
    )
puts("===============================================")
```

2. Write a method that takes an integer `n` in; it should return
`n*(n-1)*(n-2)*...*2*1`. Assume n >= 0.

```ruby
puts("\nTests for #factorial")
puts("===============================================")
    puts(
      'factorial(0) == 1: ' + (factorial(0) == 1).to_s
    )
    puts(
      'factorial(1) == 1: ' + (factorial(1) == 1).to_s
    )
    puts(
      'factorial(2) == 2: ' + (factorial(2) == 2).to_s
    )
    puts(
      'factorial(3) == 6: ' + (factorial(3) == 6).to_s
    )
    puts(
      'factorial(4) == 24: ' + (factorial(4) == 24).to_s
    )
puts("===============================================")
```

3. Write a method that takes in an integer `num` and returns the sum of
all integers between zero and num, up to and including `num`.

```ruby
puts("\nTests for #sum_nums")
puts("===============================================")
    puts('sum_nums(1) == 1: ' + (sum_nums(1) == 1).to_s)
    puts('sum_nums(2) == 3: ' + (sum_nums(2) == 3).to_s)
    puts('sum_nums(3) == 6: ' + (sum_nums(3) == 6).to_s)
    puts('sum_nums(4) == 10: ' + (sum_nums(4) == 10).to_s)
    puts('sum_nums(5) == 15: ' + (sum_nums(5) == 15).to_s)
puts("===============================================")
```

4. Write a method that takes an array of letters and returns the number
of vowels in the string. You may assume that all the letters are
lowercased. You can treat "y" as a consonant.

```ruby
puts("\nTests for #count_vowels")
puts("===============================================")
    puts('count_vowels("abcd") == 1: ' + (count_vowels('abcd') == 1).to_s)
    puts('count_vowels("color") == 2: ' + (count_vowels('color') == 2).to_s)
    puts('count_vowels("colour") == 3: ' + (count_vowels('colour') == 3).to_s)
    puts('count_vowels("cecilia") == 4: ' + (count_vowels('cecilia') == 4).to_s)
puts("===============================================")
```

5. Write a method that takes an array of letters and returns true if it
is a palindrome. A palindrome is a string that is the same whether written
backward or forward. Assume that there are no spaces; only lowercase
letters will be given.

```ruby
puts("\nTests for #palindrome?")
puts("===============================================")
    puts('palindrome?("abc") == false: ' + (palindrome?('abc') == false).to_s)
    puts('palindrome?("abcba") == true: ' + (palindrome?('abcba') == true).to_s)
    puts('palindrome?("z") == true: ' + (palindrome?('z') == true).to_s)
puts("===============================================")
```

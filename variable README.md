# Introduction to Variables

##Objectives

1. Define a variable.
2. Create and reassign variables.
3. Define pass-by-value as it relates to variables

## Video

<iframe width="960" height="720" src="https://www.youtube.com/embed/FsVYkcOoI8Y?rel=0&amp;showinfo=0" frameborder="0" allowfullscreen></iframe>

[Download MP4](http://learn-co-videos.s3.amazonaws.com/ruby/about-variables-ruby.mp4)

## Variables in Ruby

Much like in math, variables are words or characters that hold values. In algebra, however, variables are only placeholders for numbers. In Ruby, a variable can point to almost any type of value including numbers, strings, arrays, and hashes.

## Creating Variables

Variables are assigned values using `=` ("equal sign"), called the assignment operator. Variable names are typically all lower case and, in the case of multiple words, the words are separated by underscores.

```ruby
current_president = "Barack Obama"
puts "In 2014, the president was #{current_president}."
```
The code above will print `In 2014, the president was Barack Obama.`.

> Note: The syntax of `#{current_president}` simply injects the value of the variable `current_president` into the string. This is called [Interpolation](http://stackoverflow.com/questions/10076579/string-concatenation-vs-interpolation-in-ruby) and we'll cover it later - but think of it as `"In 2014, the president was" + current_president` where you are adding that value to a string.

## Reassigning Variables

Now the variable `current_president` is equal to the string Barack Obama. Let's say somehow Stephen Colbert got elected as president for 2016. To update `current_president`, you would just reassign the variable much in the same way that you first defined it:

```ruby
current_president = "Barack Obama"
puts "In 2014, the president was #{current_president}."

current_president = "Stephen Colbert"
puts "Now, it being the year 2016, the president is #{current_president}."
```
This will print out:  

```
In 2014, the president was Barack Obama.
Now, it being the year 2016, the president is Stephen Colbert.
```

## Variable Example

Within this repository is a file named `variables.rb` with some examples you can read and play with.

```ruby
'This is data, it is a string. Strings start with " "'

"Part of being data, or a string, is that ruby doesn't interpret it."

puts 1+1
puts "1+1"

example = "The word 'example' is equal to this sentence, it's a named variable."

puts example
puts example
puts example

puts "variables are any previously undefined word that"
puts "starts with a lowercase letter."
```

Running this file will print:

```bash
2
1+1
The word 'example' is equal to this sentence, it's a named variable.
The word 'example' is equal to this sentence, it's a named variable.
The word 'example' is equal to this sentence, it's a named variable.
variables are any previously undefined word that
starts with a lowercase letter.
```

## Resources

- [ZetCode Ruby Variables](http://zetcode.com/lang/rubytutorial/variables/)
- [Wikibooks: Ruby Programming/Syntax/Variables and Constants](http://en.wikibooks.org/wiki/Ruby_Programming/Syntax/Variables_and_Constants)
- [RubyMonk on Interpolation of Variables in Strings](https://rubymonk.com/learning/books/1-ruby-primer/chapters/5-strings/lessons/31-string-basics)

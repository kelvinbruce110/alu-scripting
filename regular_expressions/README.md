# Regular Expressions

This project is an introduction to **regular expressions (regex)** using **Ruby** and the **Oniguruma** regular expression library.

The goal of this project is to practice creating and using regular expressions to search for and match specific patterns in text.

## Requirements

* Ubuntu 20.04 LTS
* Ruby
* Oniguruma regular expression library
* Allowed editors:

  * `vi`
  * `vim`
  * `emacs`

## Project Structure

```text
regular_expressions/
├── README.md
├── 0-simply_match_school.rb
├── 1-repetition_token_0.rb
├── 2-repetition_token_1.rb
├── 3-repetition_token_2.rb
├── 4-repetition_token_3.rb
├── 5-beginning_and_end.rb
├── 6-phone_number.rb
├── 7-OMG_WHY_ARE_YOU_SHOUTING.rb
└── ...
```

## How the Scripts Work

Each Ruby script accepts a string as a command-line argument and uses a regular expression to find specific patterns within that string.

The general structure provided for the project is:

```ruby
#!/usr/bin/env ruby
puts ARGV[0].scan(/REGEX/).join
```

Where:

* `ARGV[0]` contains the first command-line argument.
* `scan()` searches the string for matches to the regular expression.
* `join` combines the matches into a single string.
* `puts` prints the result.

## Example

For example, the following command:

```bash
./0-simply_match_school.rb "Best School"
```

uses a regular expression to find `School` in the provided string.

Expected output:

```text
School
```

If the input contains multiple matches:

```bash
./0-simply_match_school.rb "School Best School"
```

The output is:

```text
SchoolSchool
```

## Regular Expression Concepts

Throughout this project, I will practice different regex concepts, including:

* Literal character matching
* Character classes
* Repetition
* The `*` quantifier
* The `+` quantifier
* The `?` quantifier
* Character ranges
* Beginning and end anchors
* Escaping special characters
* Matching phone numbers
* Working with uppercase and lowercase characters

## Testing

The scripts can be executed directly from the terminal.

For example:

```bash
./0-simply_match_school.rb School
```

To make a script executable:

```bash
chmod +x filename.rb
```

The scripts can also be tested using `cat -e` to make the output and ending newline visible:

```bash
./0-simply_match_school.rb School | cat -e
```

## Learning Resources

The project resources include:

* Regular expressions basics
* Regular expressions advanced concepts
* Rubular
* Interactive regular expression exercises
* Additional material about the challenges of using regular expressions

## Author

**Bruce Mupenzi**

African Leadership University


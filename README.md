# regex course

## 1. Regex Intro

### What are Regular Expressions?

REGEX are character patterns that allow you to filter data matching the pattern.

[REGEX 101 ==>](https://regex101.com/)

## 2. Language

### Predefined classes: . \d \w \s

- **.**: find all character inside file.
- **Digit**:
  - **\d**: find all number digits **(0,1, ,9)**
  - **[0-9]**: find all number digits on strict way
- **Word**:
  - **\w**: find all letters **(A, , ,Z,\_)** and number digits **(0,1, ,8,9)**
  - **[a-z]**: find all Lowercase letters on strict way
  - **[A-Z]**: find all Uppercase letters on strict way
  - **[a-zA-Z]**: find all Lowercase and Uppercase letters on strict way
  - **[a-zA-Z0-9]**: find all Lowercase, Uppercase letters and number digits on strict way
  - **[a-zA-Z0-9_]**: find all Lowercase, Uppercase letters, number digits and underscore on strict way
  - **[a-zA-Z0-9_\.]**: find all Lowercase, Uppercase letters, number digits, underscore and character DOT on strict way
- **Spaces**: normal space, tab, double space, etc
  - **\s**: find all spaces

**challenge: find a system to get all hexadecimals**
=> [#][a-fa-f0-9]{3,6}
=> [#][a-fa-f0-9]

### Delimiters: + \* ?

- **\***: greedy (get all)
- **+**: one or more
- **?**: zero or one

### Counters {Nmin,Nmax}

### Not (ˆ) Inverse/Reverse

Challenge: ([0-9]{2,2}[\W]?){3}

When we want to match all entire line text we use **ˆ** and **$**

- Start line is marked with: **ˆ**
- End line is marked with: **$**

Example: `^\d{3,6}$`

## 3. Practical cases

### Logs

- https://generatedata.com/generator

# RegEx Date Pattern

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

### Table of Contents

- [Oveview](#Overview)
- [Expression](#Expression)
- [Expression-Breakdown](Expression-Breakdown)
- [Quantifiers](#Quantifiers)
- [Optional Flags](#Optional-Flags)
- [Contributions](#Contributions)
- [Contact](#Contact-Me)

### Summary

In this quick tutorial we will look at a basic regular expression or as it sometimes called a rational expression for Dates following the format DD/MM/YYYY. DD and MM can be one or two digits. Validating dates can become quite complex so for now we just look at the initial identification of a date in a common format.

## Expresison

Below is the Reg-Ex exression we will be looking into:

`^\d{1,2}\/\d{1,2}\/\d{4}$`

## Expression-Breakdown

1. `^`the first character is a caret and this asserts position at start of a line.

2. `\d ` next we have `\d ` Here we indicate a match of any digit between 0-9.

3. `{1,2}` – This is a condition for the `\d ` digit search. It enables match of one OR two digits anywhere in sequence as many times as needed. This is called greedy regex quantifier.

4. `\/ `- the ‘\’ is a selector and the ‘/’is a match for the character `/ ` this search is case sensitive. For Example, ‘\A’

5. Repeat steps 2 and 3 for the month `\/d{1,2}\/`

6. `d{4}` similar to `d{1,2}` only it will look for 4 numbers anywhere in sequence as many times as needed (greedy quantifier).

7. `$` this asserts position at the end of the line

## Quantifiers

There are alot of quantifiers to explore and we will just look at the ones related to this search.

### Greedy

Match as many instances of the token or substring as possible. Such as when we look at `\d{1,2}`

### Lazy

In contrast to Greedy, Lazy will stop search after its first match of a date.

## Optional-Flags

Flags, in a regular expression, are tokens that modify its behavior of searching

### Global pattern flags

`g modifier: global` All matches (don't return after first match)

`m modifier: multi line` Causes `^ `and `$` to match the begin/end of each line (not only begin/end of string)

## Contributions

This is currently my own work. Please feel free to submit your contributions on GITHUB with credits given

## Contact-Me

If you have any questions or want to keep up with my latest projects, please follow me on [Github](http://www.github.com/operationBrass) or contact me via [Email](mr.brn.lewis@outlook.com).

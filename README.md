# RegEx Date Pattern

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

### Table of Contents

- [Oveview](#Overview)
- [Expression](#Expression)
- [Expression-Breakdown](Expression-Breakdown)
- [Contributions](#Contributions)
- [Questions](#Questions)

### Overview

In this quick tutorial we will look at a basic regular expression or as it sometimes called a rational expression for Dates following the format DD/MM/YYYY. DD and MM can be one or two digits. Validating dates can become quite complex so for now we just look at the initial identification of a date in a common format.

## Expresison

Below is the Reg-Ex exression we will be looking into:

`^\d{1,2}\/\d{1,2}\/\d{4}$`

## Expression-Breakdown

1. `^`the first character is a caret and this asserts position at start of a line.

2. `\d ` next we have `\d ` Here we indicate a match of any digit between 0-9.

3. {1,2} – This is a condition for the `\d ` digit search. It enables match of one OR two digits anywhere in sequence as many times as needed. This is called greedy regex quantifier.

4. `\/ `- the ‘\’ is a selector and the ‘/’is a match for the character `/ ` this search is case sensitive. For Example, ‘\A’

5. Repeat steps 2 and 3 for the month ‘\/d{1,2}\/’

6. `d{4}` similar to `{1,2}` where it is look for 4 numbers anywhere in sequence as many times as needed (greedy).

7. `$` this asserts position at the end of the line

## Technologies Involved

Regular Expression

## Contributions

This is currently my own work. Please feel free to submit your contributions on GITHUB with credits given

## Contact Me

If you have any questions or want to keep up with my latest projects, please follow me on [Github](http://www.github.com/operationBrass) or contact me via [Email](mr.brn.lewis@outlook.com).

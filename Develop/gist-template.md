# REGEX IS LORD

Welcome to the Regex Tutorial on matching email addresses. In this tutorial, we will explore the components of a regular expression that can be used to validate and extract email addresses from text. Email addresses are commonly used for communication and data collection, and understanding how to work with them using regular expressions can be highly beneficial in various applications.

## Summary

In this tutorial, we will focus on a regular expression that can match and validate email addresses. The regex we will be using is:

/^([a-zA-Z0-9_.+-])+@[a-zA-Z0-9-]+\.[a-zA-Z0-9-.]+$/


## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)
- [Back-references](#back-references)
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)

## Regex Components

### Anchors
Anchors are used to match a specific position within the text. In our email address regex, we use two anchors: ^ and $. The ^ anchor matches the start of the string, ensuring that the email address starts at the beginning. The $ anchor matches the end of the string, ensuring that the email address ends at the end of the text.

### Quantifiers
Quantifiers define the number of occurrences of a character or group that should be matched. In our regex, the + quantifier is used after the group ([a-zA-Z0-9_.+-]). It allows one or more occurrences of any alphanumeric character, underscore, dot, plus, or minus sign in the local part of the email address.

### OR Operator
The OR operator, denoted by the vertical bar |, allows us to match one pattern or another. In our regex, we don't use the OR operator explicitly. However, we can use it to extend our email address matching capabilities. For example, to allow email addresses from two different domains.

### Character Classes
Character classes allow us to match a set of characters. In our regex, we use character classes to match specific parts of the email address. The character class [a-zA-Z0-9-] matches any alphanumeric character or hyphen in the domain name. The character class [a-zA-Z0-9-.] matches any alphanumeric character, dot, or hyphen in the top-level domain (TLD) part of the email address.

### Flags
Flags are used to modify the behavior of a regular expression. In our regex, we don't use any flags since we are performing a basic match and validation.

### Grouping and Capturing
Parentheses () are used for grouping and capturing in regular expressions. In our regex, the group ([a-zA-Z0-9_.+-]) is used to capture the local part of the email address. This group allows a combination of alphanumeric characters, underscore, dot, plus, or minus sign.

### Bracket Expressions
Bracket expressions allow us to match a single character from a set of characters. In our regex, we use bracket expressions to match specific characters within the email address. For example, [a-zA-Z0-9_.+-] matches any alphanumeric character, underscore, dot, plus, or minus sign in the local part of the email address.

### Greedy and Lazy Match
greedy matching tries to consume as much as possible, while lazy matching tries to consume as little as possible to satisfy the overall pattern. The choice between greedy and lazy matching depends on the specific requirements of your regular expression and the desired behavior for matching multiple occurrences of a pattern.

### Boundaries
Using boundaries in regular expressions allows us to define precise conditions for matches based on the positions of characters or groups within the text. They help us ensure that matches occur at specific word boundaries or at the start or end of lines, providing more control over the matching process and enabling us to create more accurate and targeted regular expressions.

### Back-references
Back-references are powerful tools in regular expressions as they allow us to match duplicated patterns and ensure consistency within the same string. They enable us to perform complex matching and manipulation of text based on previously captured groups. They are denoted by the backslash \ followed by a number or a name.

### Look-ahead and Look-behind
Look-ahead and look-behind assertions are powerful tools that allow us to impose additional conditions on our regular expressions based on the context that precedes or follows a specific position. They enable us to create more precise and complex matching patterns, making regular expressions more flexible and adaptable to various scenarios. examples are (?=) (?!) (?<=) and (?<!)

## Author

Github: Jsuttle2

Email: Jsuttle2@gmail.com

REGEX-GIST.MD EMAIL TUTORIAL

Regular expression (REGEX) is used when someone is trying to match a character combination with a string. It is good for both pulling out information from a code and being used for validation.

## Summary
This code will be used throughout the tutorial to give examples for how regex can be used. The code can be used for matching emails.
Matching email: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/


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
The anchor starts and ends the regular expression:
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/.

The anchors are the ^ and the $. This code specifically is saying that we are looking for something that starts with
^([a-z0-9_\.-]+)

We will define what everything inside the parentheses later in this tutorial, but what the anchor means is that if we are to find a match it has follow those initial guidelines. It also has to end with

.([a-z\.]{2,6})$.

So, it must start and end with the given parameters within the code. If it does not, then it is not a match.

### Quantifiers
Quantifier's determine how many times a specific character or group of characters needs to be present in order to have a match. Quantifiers in this regex includes the + operator, which will connect the users email name + email service + .com. Another quantifier for this regex includes {2,6}, which will allow a match range of 2-6 characters for the character set of [a-z\.]

### OR Operator
It is not present in the code for the given matching email code, but in order to talk about the OR Operator, we will look at the following code for matching a hex code.

/^#?([a-f0-9]{6}|[a-f0-9]{3})$/

This is a regex for matching a hex code that uses the OR Operator. What this will do is it will match where it starts with the # and that has to come first followed by one of the following:

[a-f0-9]{6} which will match a 6 character long string that contains a combination of a-f letters and 0-9 numbers.

| OR Operator

[a-f0-9]{3} it will match a 3 character long string that contains a combination of a-f letters and 0-9 numbers.



### Character Classes
The character class in this expression is \d, which matches a single characters that is a digit from 0-9. It will only match a single digit such as "4", but not "44"


### Flags
A regex flag is not used in the matching email code that is being used for this tutorial. A regular expression typically comes in the form: /regex/
Where the slashes denote where the regular expresssion starts and ends. A flag can be used after the slash to give more guidelines for our matching. The flags are:
"G" which stands for "global" which will allow for matching all the instances within a string that follow the matching guidelines set in the regular expression.
"M" which stands for "multiline" which will search line by line rather than searching through a string as a whole.
"I" which stands for "insensitive" will make the regular expression case-insensitive, so capitals and lower-case letters will not deture the matching.


### Grouping and Capturing
Capturing group #1 in this expression is ([a-z0-9_\.-]+) that matches the user email name. The second capturing group is ([\da-z\.-]+) which will match the email service. Then lastly, capture group #3 is ([a-z\.]{2,6}) to capture the .com.


### Bracket Expressions
Contininuing with the code for matching an email: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
Grouping and capturing: [a-z0-9_\.-]
The guidelines for matching the group. For this code snippet, it can contain letters a-z, numbers 0-9, an underscore, hyphen, or period. The period is an escaped character, so it requires the backslash in order to be able to be matched.


### Greedy and Lazy Match
This regrex includes greedy matches. Since it includes the + Quantifier, it will match as many times as possible giving back as needed. Another greedy Quantifier used in this regex is {} when matching `{2,6} for the last capture group.

### Boundaries
We are looking for specific words inside of a string.  Boundaries are not used in the given matching an email code.


### Back-references
Back-references are not included in the given code.


### Look-ahead and Look-behind
If using a look-ahead or look-behind, then it has to match in a certain order. It is not being used in the given matching an email code.

## Very helpful YouTube video
https://www.youtube.com/watch?v=7DG3kCDx53c

## Author
This tutorial was created by Uday Gautam and my peer Diana Portillo. 


You may contact me here:
Github: https://github.com/ugautambeast.
Email: Udaygautam77@gmail.com

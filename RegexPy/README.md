regex_py
1. Manipulation Text with Regular Expressions (remindered/recap basic information about regex)
Solution tasks: 
2.1 Problem 1
Capture words that start with a vowel letter (aeiou), but ends with a non-vowel letter. There can be 0 or more letters in between. Also, it is not allowed to have other characters besides letter in between. e.g. your regular expression should match unicorn, element, but should not match: banana, apple. All letters are lowercase.

2.2 Problem 2
Capture numbers in octal or hexadecimal representation in Python. Octal numbers start with a prefix "0o" (number zero followed by lowercase letter o), and are followed by one or more numbers in the range of 0 to 7. E.g. 0o112, 0o237, 0o07. Hexadecimal numbers start with a prefix "0x", and are followed by one or more numbers in the range of 0 to 9 or lowercase letters in the range of a to f. E.g. 0xf3, 0x1d, 0x072.

2.3 Problem 3
Capture a "Firstname Lastname" at the beginning of each line. e.g. for sentence Jane Doe is eating breakfast. Your regex should capture "Jane Doe". But in sentence Today is John Doe's birthday. Your regex should NOT capture the name in the sentence as it does not start from the beginning of the string. Notice that the name should consist of two words. Each word should start with a capital letter and has zero or more lowercase letters followed. No other symbols are allowed in the name. Some valid names are: Issac Newton, L Zhang; Some invalid names are: john doe, Ling-Ling Li.

2.4 Problem 4
In this problem, we are using re.findall. Notice that if you use normal parentheses for grouping, re.findall only returns the value in the group but does not return the complete matched string. Match any price in the form  3.45𝑜𝑟
 23.32 or $400.

2.5 Problem 5
Capture email address with letters, numbers, underscore and dots. A valid email address defined in this problem must meet the following requirements:

- Has an "@" symbol;
- Before the "@" symbol, there can be one or more strings made of letters, numbers and underscores, separated by a single dot.
- After the "@" symbol, there can two or more strings made of letters, numbers and underscores, separated by a single dot.
- No other characters besides letters, numbers, underscores, dots, and the "@" symbol should appear in the email address.

2.6 Problem 6
What is the correct regular expression to match a URL with letters, numbers, underscores and dots? A valid URL defined in this problem must meet the following requirements:

- The URL consists of two or more strings made of letters, numbers, and underscores.
- A dot is used in between the strings.
- No two dots are allowed to appear consecutively.

2.7 Problem 7 
What is the correct regular expression to match an ISBN number from two publishers (World Scientific from Singapore, and Sigma Publications from Greece)? A valid ISBN code defined in this problem must meet the following requirements:

- The ISBN number consists of 10 digits, with dashes(-) in between.
- The ISBN number must match the patterns of one of the following publishers(x means a digit from 0 to 9): for World Scientific, the pattern should be xxxx-x-xxxx-x, and for Sigma Publications, the pattern should be xxx-xxx-xxx-x.

2.8 Problem 8
What is the correct regular expression to match a DOI registered by Crossref? A valid DOI(e.g. doi:10.1038/nphys1170) defined in this problem must meet the following requirements:

- The DOI starts with doi:
- The link has two parts divided by a “/”. In the first part, there can only be numbers and dots, and in the second part, there can be any characters. There should be at least one character in each part.

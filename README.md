# bbcc_BuggyCompliance
programming exercise

A Compliance Problem

Introduction
As part of a team project to build an instant messaging program, you have to work around your
teammate's buggy compliance filter.

The compliance filter works based on an algorithm which determines if certain messages can pass
through the system and if they should be flagged. Usually the compliance filter system has a dictionary
of black listed words which it filters out.

However, due to your teammate's programming error the compliance filter system appears to only allow
words that are palindromes or anagrams of palindromes (i.e. can make a palindrome when re-arranged).

For example:
abba
aabb (this one is an anagram of abba or baab)
civic
deified
mom
mmo
radar

While a fix is being worked on, you are tasked with writing an add on that will determine if a word can
pass through the this system.

Input Specifications
Your program will take
A string S denoting the word to be tested. All letters in the alphanumeric input will be lowercase
(1 ≤ LENGTH(S) ≤ 500), and there may be numbers and symbols.

Output Specifications
Based on the input,
Print out yes if the input would pass through the system
Print out no if the input would fail the system

Sample Input/Output
Input
abba
Output
yes
Explanation
abba is already a palindrome.

Input
nnmm
Output
yes
Explanation
While nnmm isn't a palndirome, it can be re-arranged to make one; nmmn and mnnm are palindromes
that can pass through the system.

Input
trail
Output
no
Explanation
trail isn't a palindrome, nor an anagram of a palindrome, and therefore will not pass through the system.

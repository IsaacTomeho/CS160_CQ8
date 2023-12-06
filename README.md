# CS160_CQ8

Staircase:\
Space Complexity - O(1)\
Time Complexity - O(n^2)\

Alternating Characters:\
Space Complexity - O(n)\
Time Complexity - O(n)\

Recursive Definition:\
Base Case: If s is empty or has only one character (s.length() <= 1), return 0. This is since no deletions are required for a string of length 0 or 1.\
Recursive Case: If the first two characters of s are the same (s.charAt(0) == s.charAt(1)), one character must be deleted.\
Therefore, return 1 + alternatingCharacters(s.substring(1)), which represents one deletion plus the number of deletions required for the rest of the string.\
If the first two characters are different, no deletion is required at this step.\
Therefore, return alternatingCharacters(s.substring(1)), which evaluates the number of deletions required for the rest of the string.\

```

FOR alternative POSIX notation:
https://github.com/micromatch/posix-character-classes

Character classes

.           - Matches any character except newline
\d          - Digit (0-9)
\D          - Not a digit (0-9) - opposite of \d
\w, [A-Za-z0-9_], [:word:]   - Word character (a-z, A-Z, 0-9 and _)
\W, [^A-Za-z0-9], [^:word:]  - Not a word character
\s          - Whitespace (space, tab, newline)
\S          - Not whitespace (space, tab, newline) - opposite of \s
[]          - Matches characters in brackets
[^ ]        - Matches characters NOT in brackets
[a-z]       - lowercase characters or [:lower:] in POSIX notation
[A-Z]       - uppercase characters or [:upper:] in POSIX notation
[a-zA-Z]    - lowercase and uppercase characters or [:alpha:] in POSIX notation

Anchors
\b      - Word boundary
\B      - Not a word boundary - opposite of \b
^       - Start of a string (or start of line in multiline pattern)
$       - End of a string (or end of line in multiline pattern)
|       - Either Or
( )     - Group

Quantifiers:

*       - 0 or More
    eg: ab*     - where b is optional (if present, must match 1 or more)
+       - 1 or More
    eg: ab+     - where the character b pattern must be present (or required) 1 or more
?       - 0 or 1
    eg: ab?     - where the character b pattern is optional (if present only 1 character is required)
{N}     - Exactly N, where N usually a number
    eg: {3}     - Exactly 3
{N,}    - N or more
    eg: {3,}    - 3 or more
{MIN_N,MAX_N}   - Range of Numbers (Minimum, Maximum)
    eg: {3,5}   - Minimum of 3 and maximum of 5
```

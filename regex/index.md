# Some small thing about regex I studied

- Metacharacters
	- Period character `.`: match **any** character
	- Caret sign `^`: causes the match to occur only if the regular expression is
	found at the **beginning** of the line
	- Dollar sign `$`: causes the match to occur only if the regular expression is
	found at the **end** of the line
	- Alternation `a|b`: match **either the string a or the string b** and not limited to 2 choices
	- Quantifiers
		- `?`: match an element **zero** or **one** time
		- `*`: match an element **zero** or **more** times
		- `+`: match an element **one** or **more** times
		- `{x}`: match an element **exactly x** time(s)
		- `{x,y}`: match an element **x to y** times
		- `{x,}`: match an element **x or more** times
		- `{,y}`: match an element **y or fewer** times
	- Bracket `[abc]`: matches **a single character** from **a specified set of characters**
		- In bracket, metacharacters lose their special meaning, but there are two cases in which metacharacters are used within bracket expressions and have different meanings
			- Negation `^` : opposed to normal bracket, it **wont** match a single character from a specified set of characters
			- Dash `-`: indicate a character range like `a-z`, `A-Z`, `0-9`

- Character classes
	- `[:alnum:]`: the alphanumeric characters, equivalent to `[A-Za-z0-9]`
	- `[:word:]`: `[:alnum:]` with the addition of the underscore character `_`
	- `[:blank:]`: the space and tab characters
	- `[:alpha:]`: the alphabetic characters, equivalent to `[A-Za-z]`
	- `[:cntrl:]`: the ASCII control codes including the ASCII characters 0 through 31 and 127
	- `[:digit:]`: equivalent to `[0-9]`
	- `[:graph:]`: the visible characters including characters 33 through 126
	- `[:punct:]`: the punctuation characters, equivalent to `[-!"#$%&'()*+,./:;<=>?@[\\\]_{|}~]\`
	- `[:space:]`: equivalent to `[ \t\r\n\v\f]`
	- `[:xdigit:]`: characters used to express hexadecimal numbers, equivalent to `[0-9A-Fa-f]`
	- `[:print:]`: printable characters, including all characters in `[:graph:]` plus the space character
	- `[:lower:]`: equivalent to `[a-z]`
	- `[:upper:]`: equivalent to `[A-Z]`

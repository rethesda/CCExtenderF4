# Table of Contents

* [Build Dependencies](#build-dependencies)
* [End User Dependencies](#end-user-dependencies)
* [Console commands](#console-commands)
	* [Help](#help)
	* [Clear](#clear)

# Build Dependencies
* [Boost](https://www.boost.org/)
	* Algorithm
	* Container
	* Iterator
* [CommonLibF4](https://github.com/Ryan-rsm-McKenzie/CommonLibF4)
* [robin-hood-hashing](https://github.com/martinus/robin-hood-hashing)

# End User Dependencies
* [Microsoft Visual C++ Redistributable for Visual Studio 2019](https://support.microsoft.com/en-us/help/2977003/the-latest-supported-visual-c-downloads)
* [F4SE](https://f4se.silverlock.org/)

# Console Commands

## Help

**Command**: `"Help" <expr>`  
**Description**: Performs a substring search on all forms by (override) name and editor ID. This reimplementation is noticably faster and more accurate than the original version.  
**Example Usage**: `help laser 4 weap`  
**Grammar**:
```
<expr> ::= <empty> | " " <matchstring> | " " <matchstring> " " <filter> | " " <matchstring> " " <filter> " " <form-type>
<matchstring> ::= <string> ; The string to filter results with
<filter> ::= <integer>
	; 0 - All
	; 1 - Functions
	; 2 - Settings
	; 3 - Globals
	; 4 - Forms
<form-type> ::= <string> ; The form type to filter form results with
```

## Clear
**Command**: `"Clear"`  
**Description**: Clears the console output.  
**Example Usage**: `clear`

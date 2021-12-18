# LOLCODE

LOLCODE is an esoteric programming language inspired by lolcat inernet memes. The language was created in 2007 by Adam Lindsay, a year after LOLCATS ebcame an Internet meme.

## LOLCODE Basics
### Syntax
``` php
    HAI 1.2
        your code here
    KTHXBYE
```

1.2 is a LOLCODE Language Specificaiton Version Number. KTHXBYE is short for *"Okay, Thanks, Bye"*

### Variables and Variable Types
LOLCODE is a dynamically typed language. Variables don't have fixed types. A variable's type is the same as the type of value it is currently storing.
``` php
    I HAS A varName ITZ value //declare and assign in the same step
    I HAS A x ITZ 3 //declare x with value 3

    varName R value //assign to a variable
    x R 4 //assigns value 4 to x
```
In naming variables:
- It must begin with a Letter
- It can contain Letters, Numbers, Underscores
- It cannot use Dashes or any other Special Characters
- It can use Lowercase or Uppercase, or a Combination of Both

***Note*** *: LOLCODE is case-sensitive. Thus, variable names are also case sensitive*
| type  | in LOLCODE   |
|----------|--------|
| strings  | YARN   |
| integers | NUMBR  |
| floats   | NUMBAR |
| booleans | TROOF  |

### Comments
- **BTW** *(By The Way)* is used for a single-line comment.
- **OBTW** *(Oh By The Way)* starts a multi-line comment while **TLDR** *(Too Long, Didn't Read)* ends a multi-line comment.

### Operators
| operator    | function                    | syntax             |
|-------------|-----------------------------|--------------------|
| SUM OF      | addition                    | SUM OF x AN y      |
| DIFF OFF    | subtraction                 | DIFF OF x AN y     |
| PRODUKT OF  | multiplication              | PRODUKT OF x AN y  |
| QUOSHUNT OF | division                    | QUOSHUNT OF x AN y |
| MOD OF      | modulo                      | MOD OF x AN y      |
| BIGGR OF    | maximum between two numbers | BIGGR OF x AN y    |
| SMALLR OF   | minimum between two numbers | SMALLR OF x AN y   |
**AN** Keyword is not required when using Unary Operators.
- If both argumetns are **NUMBR**, result is Integer.
- If one of the numbers is a **NUMBAR**,  result will be a float.
- Interpreter will try to automatically cast your argumetns to numbers. If argument cannot be cast, an error will be raised

### Booleans
| operation   | function                    | syntax             |
|-------------|-----------------------------|--------------------|
| AND         | and function                | BOTH OF x AN y     |
| OR          | or function                 | EITHER OF x AN y   |
| XOR         | xor function                | WON OF x AN y      |
| NOT         | unary negation              | NOT x              |

### I/O
- **GIMMEH**
    ```php
        HAI 1.2
           GIMMEH x
           BTW stores input to x as a YARN 
        KTHXBYE
    ```
- **VISIBLE**
    ```php
        HAI 1.2
           GIMMEH x
           VISIBLE x
           BTW prints x as a YARN 
        KTHXBYE
    ```
```php
    HAI 1.2
        GIMMEH x
        x IS NOW A NUMBR, BTW x is now an integer
        VISIBLE x
        BTW prints x as a NUMBER 
    KTHXBYE

    or

    HAI 1.2
        GIMMEH x
        MAKE x A NUMBAR, BTW x is now a float
        VISIBLE x
    KTHXBYE    
```

### IF-THEN STATEMENTS
- it is similar to if-else statements in C and Java.
The general form is
```php
	<any_expression>
	O RLY?
		YA RLY
			<code to execute if above condition is true>
		NO WAI
			<code to execute in this block>
	OIC
```
There are 4 keywords used such as 'O RLY', 'YA RLY', 'NO WAI', and 'OIC'.
- O RLY is like the start of the statement.
- YA RLY is similar to if-statement
- NO WAI is similar to else-statement
- OIC is the end of statement.

There is an optional keyword that is used between YA RLY and NO WAI which is called MEBBE.
- If the YA RLY condition is satisfied, the MEBBE keyword will be executed if MEBBE is TRUE.

### CASE STATEMENTS
```php
	WTF?
		OMG <any value to compare>
			<code block to execute if expression is satisfied>
		OMG <any value to compare>
			<code block to execute if expression is satisfied>
		OMGWTF
			<code block to execute as a default case>
	OIC
```
- The WTF? keyword is similar to switch.
- The OMG keyword is a comparison block in which it should be a literal.
- Every OMG block must be terminated with a GTFO statement. 
- If none of the literals are true, a default case is used with the keyword 'OMGWTF'.


### LOOPS
The iteration loops have the following structure:
```php
	IM IN YR <label> <any_operation> YR <any_variable> [TIL|WILE <expression>]
		<code block to execute inside the loop multiple times>
	IM OUTTA YR <label>
```
- note that inside the funnction body, particularly in <any_operation>, UPPIN means increment by one and NERFIN means decrement by one.
- The TIL keyword is used if the statement evaluates as FAIL, the loop continues, otherwise the loop will stop. 
- On the other hand, the WILE keyword is the exact opposite of TIL. If the statement evaluated as WIN(condition is satisfied), the loop continues, otherwise it would stop.

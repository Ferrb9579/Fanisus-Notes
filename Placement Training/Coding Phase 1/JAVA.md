## What is a Data Type?
A **data type** defines the type of data a variable can store.  

---

## Data Types in Java
- **Primitive Data Types**
- **Non-Primitive Data Types**

---

## Primitive Data Types

1. **Boolean**
   - `boolean` (1 bit)

2. **Character**
   - `char` (2 bytes)

3. **Integer Types**
   - `byte` (1 byte)
   - `short` (2 bytes)
   - `int` (4 bytes)
   - `long` (8 bytes)

4. **Floating-Point Types**
   - `float` (4 bytes)
   - `double` (8 bytes)

---

## Non-Primitive Data Types
- Array  
- Class  
- Interfaces  
- String  
- Enum  

---

## Examples

- If data is `100`, where will you store this data?  
  ```java
  byte a = 100;
  ```

## Default Datatypes
* Int
* Double

## Type Casting
### Explicit
In narrowing pr

```java
byte a = (byte) 129;
```
### Implicit



## Binary Addition
0 1 1 1 1 1 1 1 1
0 0 0 0 0 1 0 1 0 (+)
____________
1 0 0 0 0 1 0 0 0

## Operation on numbers
By default the number is converted from byte, short, char to int for calculation

Whenever we perform actions on variables default assumption will be integers, depends on the destination type casting might be needed

Whenever we perform operation on direct values, we get the desired output if it is in the range type casting might be needed



Numerator = (Denominator X Quotient) + Remainder


(2 < 3) && (3 < 5)




### Byte
```java
byte a = 10;
a = (byte)(a + 5); // Explicit Type Casting
a += 5; // Implicit Type Casting
System.out.println(a);
```


### Increment and Decrement

a++
++a
a--
--a

* Update the value
* If pre return updated value else post return old value

```java
int a - 10;
int x = ++a + ++a;
System.out.println(x) // 23
```




```java
byte x = 127;
int z = x++;
-128 127
```


### Bitwise operator
&
1 0 1 0
0 0 1 0 (&)
_____

|
1 0 1 0
0 0 1 0
_____
1 0 1 0

20 & 1
1 0 1 0 0
0 0 0 0 1
0 0 0 0 0

20 ^ 0
1 0 1 0 0
0 0 0 0 0
_______
1 0 1 0 0

20 ^ 1
1 0 1 0 0
0 0 0 0 1
_______
1 0 1 0 1

### Variable Swapping
```java
int a = 5;
int b = 10;
a = a ^ b;
b = a ^ b;
a = a ^ b;
```
a = 0 1 0 1
b = 1 0 1 0
a = 1 1 1 1
b = 0 1 0 1
a = 1 0 1 0




### Operators
Postfix (expr++, expr--)
Unary (++expr, --expr, +expr, -expr, ~, !)
Multiplicative (\*, /, %)
Additive (+, -)
Shift (<<, >>, >>>)
Relational (<, >, <=, >=, instanceof)
Equality (\==, !=)
Bitwise AND  ()
Bitwise Exclusive OR
Bitwise Inclusive OR
Logical AND
Logical OR
Ternary
Assignment




5 + 7 - 2 % 4 \* 3 / 4
5 + 7 - 1.5
10.5


### Associativity
* Left to Right
* Right to Left

### Control Flow Statements
Statements which are used to control the flow of execution

* Conditional
	If 
	If-Else
	Else-If-Else
	Nested
* Looping
	For
	While
	Do-While

Curly brackets are used for block of code

For if, else the curly braces is optional


```java
public static void tellAge() {
	System.out.println(19);
}

```


### Issue of nextLine
```java
Scanner s = new Scanner(System.in);
long number = s.nextLong();
String name = s.nextLine();
```

Here the name contains \n character got from previous input so we can avoid this by below code

```java
Scanner s = new Scanner(System.in);
long number = s.nextLong();
s.nextLine();
String name = s.nextLine();
```

---
* Natural Statement
	These are statement that are not in the conditional block
* Selective statement 
	These are statements that are inside a conditional code block
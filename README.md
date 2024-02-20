# Java Learning
## Java 17 Installation

Download Java 17 from 
> https://www.oracle.com/java/technologies/

Get the right installer for the machine.

## JShell

Type ``jshell`` in terminal, it will work like Jupyter Notebook where each command is stored in memory and can executed next

## IntelliJ

Advanced IDE (Integrated Development Environment) which would increase developer productivity while writing code.

Download IntelliJ from
> https://www.jetbrains.com

## Java Primitive Type
**Whole Number**
Type | Byte | Minimum | Maximum
--- | --- | --- | ---
byte | 1 | -128 | 127
short | 2 | -32768 | 32767
int | 4 | -2147483648 | 2147483647
long | 8 | -9223372036854775808 | 9223372036854775807

There is a chance of overflow and underflow happening when addition and subtraction is not well controlled in the code. Example added 1 to Integer.MAX_VALUE would result to -2147483648. Which is absolutely wrong in this context. Hence, choosing the right data type is very important.

For ``long``, we would need to add 'l' or 'L' (recommeded as it doesn't looks like 1) suffix to the back of the number to tell the compiler its a long value. Otherwise compiler would treat the it as ``int`` by default.

**Decimal**
Type | Byte | Minimum | Maximum
--- | --- | --- | ---
float | 4 | 1.4E-45 | 3.4028235E38
double | 8 | 4.9E-324 | 1.7976931348623157E308

For ``float``, we would need to add 'f' or 'F' suffix to the back of the number to tell the compiler its a ``float`` value. Otherwise the compiler would treat it as a ``double``.

For ````double``, we would need to add 'd' or 'D' suffix to the back of the number to tell the compiler its a ``double`` value. Since ``double`` is default by java, the suffix is optional

**Character**
Type | Byte
--- | --- 
char | 2 

**Boolean**
Type | Bit
--- | --- 
boolean | 1

**String**
String is not a primitive but often associated as primitive type as it is one of the frequenly used class. String is immutable and able to store chain of characters. 

## Operators
**Generic**
Operator | numeric | char | boolean | String
--- | --- | --- | --- | ---
\+ | Addition | Addition | n/a | Concatenation
\- | Substraction | Substraction | n/a | n/a
\* | Multiplication | Multiplication | n/a | n/a
/ | Division | Division | n/a | n/a
% | Remainder | Remainder | n/a | n/a

% is called as ``modulus`` which return remainder in division.

**Abbreviating Operator**
Shorthand Operator | Sample
--- | ---
Pre-fix Increment Operator | ++result;
Pre-fix Decrement Operator | --result;
Post-fix Increment Operator | result++;
Post-fix Decrement Operator | result--;
Addition Compount Assignment | result += 5;
Subtraction Compound Assignment | result -= 5;
Multiplication Compound Assignment | result *= 5;
Division Compound Assignment | result /=5;

Post-fix operator will only increment the value after code execution, hence while assigning a value with post-fix increment, the value will not incremented yet. Upon completion of value assignment, the value will be incremented.
# JAVA BASIC 

## Variables

The Java programming language defines the following kinds of variables:
1. Instance Variables (Non-Static Fields) :fields declared without the **static** keyword and it's called **instance variables** because their values are unique to each instance of a class
2. Class Variables (Static Fields)
3. Local Variables
4. Parameters

### Naming
1. Variable names are case-sensitive
2. Subsequent characters may be letters, digits, dollar signs, or underscore characters.
3. If the name you choose consists of only one word, spell that word in all lowercase letters. If it consists of more than one word use the camel case way to write

## Operators


Operator | Precedence
---------|------------ 
postfix	 |expr++ expr--
unary	 |++expr --expr +expr -expr ~ !
multiplicative |	* / %
additive |	+ -
shift	|<< >> >>>
relational |	< > <= >= instanceof
equality   |	== !=
bitwise AND|	&
bitwise exclusive OR	|^
bitwise inclusive OR	||
logical AND	|&&
logical OR	|||
ternary	|? :
assignment |	= += -= *= /= %= &= ^= |= <<= >>= >>>=

## Expressions, Statements, and Blocks

### Expressions
An expression is a construct made up of variables, operators, and method invocations, which are constructed according to the syntax of the language, that evaluates to a single value.
> example: 10/( 2 + 8 ) 

### Statements

Statements are roughly equivalent to sentences in natural languages. A statement forms a complete unit of execution.

~~~
// assignment statement
aValue = 8933.234;
// increment statement
aValue++;
// method invocation statement
System.out.println("Hello World!");
// object creation statement
Bicycle myBike = new Bicycle();
~~~

### Blocks
any statements between two curly braces

## Control Flow Statements

theres types of control statement such as 
1. decision-making statements  (if-then,if-then-else,switch )
2. looping statements (for, while, do-while)
3. branching statements (break, continue, return)

### if-then statement 
 tells your program to execute a certain section of code only if a particular test equal true
 ### if-then-else statement 
 it will execute if statement if true and if it false it will execute else statement

 ### switch

 ~~~
    int month = 5;
    String monthString;
    switch (month) {
        case 1:  monthString = "January";
                    break;
        case 2:  monthString = "February";
                    break;
        case 3:  monthString = "March";
                break;
        case 4:  monthString = "April";
                break;
        default: monthString = "Invalid month";
                 break; 
~~~

 ### while & do-while
 ~~~
while (true){
    System.out.println("true")
}
infinite loop
--------------

do {
     statement(s)
} while (expression);
~~~

### for loop 

~~~
class EnhancedForDemo {
    public static void main(String[] args){
         int[] numbers = 
             {1,2,3,4,5,6,7,8,9,10};
         for (int item : numbers) { //or for (int i=0 ; i<=10; i++)
             System.out.println("Count is: " + item);
         }
    }
~~~

###  break Statement
```
for (i = 0; i < arrayOfInts.length; i++) {
            if (arrayOfInts[i] == searchfor) {
                foundIt = true;
                break;
            }
        }
```

### continue Statement
~~~
 test:
        for (int i = 0; i <= max; i++) {
            int n = substring.length();
            int j = i;
            int k = 0;
            while (n-- != 0) {
                if (searchMe.charAt(j++) != substring.charAt(k++)) {
                    continue test;
                }
            }
~~~

### return 
* The return statement exits from the current method, and control flow returns to where the method was invoked.

* When a method is declared void, use the form of return that doesn't return a value.
retutn;

* to return a value  use return y;



# what is compile code
the compilor (usually another program) takes the program the human wrote, and converts it into the program the computer can understand whiches bunch of 0's and 1's code 

# Making Sense of Java’s API Documentation
You can find things in the API documentation in a number of different ways
1. using the index 
2. Using the list of classes


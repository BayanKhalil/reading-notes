
# Java Type System

In java Every primitive type like int, boolean, corresponds to a reference typ like <Integer>, <Boolean>, etc
```
Integer j = 1;          // autoboxing converted from primitive to reference type
int i = new Integer(1); // unboxing converting from reference type to primitive 
```

## Single Item Memory Footprint

the primitive type variables have the following impact on the memory:
```
boolean – 1 bit
byte – 8 bits
short, char – 16 bits
int, float – 32 bits
long, double – 64 bits
```
> The primitive type live on the stack and The reference types are objects, they live on the heap and are relatively slow to access

```
Boolean – 128 bits
Byte – 128 bits
Short, Character – 128 bits
Integer, Float – 128 bits
Long, Double – 192 bits
```
## Memory Footprint for Arrays
```
long, double: m(s) = 128 + 64 s
short, char: m(s) = 128 + 64 [s/4]
byte, boolean: m(s) = 128 + 64 [s/8]
the rest: m(s) = 128 + 64 [s/2]
```
> arrays of the primitive types long and double consume more memory than their wrapper classes Long and Double.

> either that single-element arrays of primitive types are almost always more expensive (except for long and double) than the corresponding reference type.

## Performance

it depends very much on the hardware on which the code runs, on the compiler that might perform certain optimizations, on the state of the virtual machine, on the activity of other processes in the operating system.

## Default Values
the primitive types may acquire values only from their domains, while the reference types might acquire a value (null) that in some sense doesn't belong to their domains.so for that isn't considered a good practice to leave variables uninitialized because it already have space in
memory

All of this information will help us when we creating API and  When our application needs collections with a big number of elements, we should consider using arrays with as more “economical” type as possible.








# What Is an Exception?
 An exception is an event, which occurs during the execution of a program, that stop the normal flow of the program's instructions

 exception objec: it's an object created by amethod to hand error off to the runtime system  it will contains information about the error 

 throwing an exception: Creating an exception object and handing it to the runtime system

 call stack :list of methods that had been called to get to the method where the error occurred

 exception handler: block of code that can handle the exception that contained in method that run time system search about

 # The Catch or Specify Requirement
 This means that code that might throw certain exceptions must be enclosed by either of  these method
 1.  try statement that catches the exception
 2. method that specifies that it can throw the exception

 ## Three Kinds of Exceptions
 1.  checked exception
 > Checked exceptions are subject to the Catch or Specify Requirement
 2. error
 > Runtime exceptions are not subject to the Catch or Specify Requirement
 3. runtime exception
 > Runtime exceptions are not subject to the Catch or Specify Requirement

 ## Catching and Handling Exceptions:
 
 **The try Block**: The first step in constructing an exception handler is to enclose the code that might throw an exception within a try block

 **The catch Block**:we  associate exception handlers with a try block by providing one or more catch blocks directly after the try block
 ```
 try {
    code
}

catch (ExceptionType name) {
    and finally blocks 
}
```



 # Scanning
 Objects of type Scanner are useful for breaking into tokens depend on their datat type 

  **Breaking Input into Tokens** :By default, a scanner uses white space to separate tokens.
  ```
  Scanner s = null;

try {
    s = new Scanner(new BufferedReader(new FileReader("xanadu.txt")));

    while (s.hasNext()) {
        System.out.println(s.next());
    }
} finally {
    if (s != null) {
        s.close();
    }
}

  ```

  > To use a different token separator, invoke useDelimiter(), specifying a regular expression.



# Read: 03 - Maps, primitives, File I/O

### Java Primitives versus Objects

###### Java Type System
Java has a two-fold type system: primitive and reference.
* primitives such as int, boolean.
* reference types such as Integer, Boolean.

The wrapper classes are immutable (so that their state can't change once the object is constructed).
* The process of converting a primitive type to a reference one is called autoboxing, the opposite process is called unboxing.

###### Pros and Cons
The decision what object is to be used is based on some reason such as :
 what application performance we try to achieve, 
how much available memory we have, 
the amount of available memory and what default values we should handle.

###### Single Item Memory Footprint
primitive type variables have the following impact on the memory:
boolean – 1 bit
byte – 8 bits
short, char – 16 bits
int, float – 32 bits
long, double – 64 bits
these values can vary depending on the Virtual Machine implementation.
Variables of these types live in the stack and hence are accessed fast. 
a single instance of a reference type on this JVM occupies 128 bits except for Long and Double which occupy 192 bits:
Boolean – 128 bits
Short, Character – 128 bits
Integer, Float – 128 bits
Long, Double – 192 bits

###### Performance
The performance of a Java code is quite a subtle issue, it depends very much on the hardware on which the code runs, on the compiler that might perform certain optimizations, on the state of the virtual machine, on the activity of other processes in the operating system.

* the primitive types are much faster and require much less memory.

* When our application needs collections with a big number of elements, we should consider using arrays with as more “economical” type as possible



### Exceptions

##### What Is an Exception?
* An exception is an event that occurs during the execution of a program that disrupts the normal flow of instructions.
* When an error occurs within a method, the method creates an object and hands it off to the runtime system.
*  Creating an exception object and handing it to the runtime system is called throwing an exception.
* The runtime system searches the call stack for a method that contains a block of code that can handle the exception.

##### The Catch or Specify Requirement
* Valid Java programming language code must honor the Catch or Specify Requirement.
* The Three Kinds of Exceptions:
1. checked exception: A well-written program will catch this exception and notify the user of the mistake, possibly prompting for a corrected file name.
2. error:  are those exceptions indicated by Error and its subclasses.
3. runtime exception:  These usually indicate programming bugs, such as logic errors or improper use of an API. For example, consider the application described previously that passes a file name to the constructor for FileReader. 

##### How to Throw Exceptions
* All methods use the throw statement to throw an exception. The throw statement requires a single argument: a throwable object. 
* Throwable objects are instances of any subclass of the Throwable class. Here's an example of a throw statement.
###### The try-with-resources Statement
* try, catch, and finally code blocks for the writeList method in the ListOfNumbers class.
Example:
public void writeList() {
    PrintWriter out = null;

    try {
        System.out.println("Entering" + " try statement");

        out = new PrintWriter(new FileWriter("OutFile.txt"));
        for (int i = 0; i < SIZE; i++) {
            out.println("Value at: " + i + " = " + list.get(i));
        }
    } catch (IndexOutOfBoundsException e) {
        System.err.println("Caught IndexOutOfBoundsException: "
                           +  e.getMessage());
                                 
    } catch (IOException e) {
        System.err.println("Caught IOException: " +  e.getMessage());
                                 
    } finally {
        if (out != null) {
            System.out.println("Closing PrintWriter");
            out.close();
        } 
        else {
            System.out.println("PrintWriter not open");
        }
    }
}

### Scanning
* Objects of type Scanner are useful for breaking down formatted input into tokens and translating individual tokens according to their data type.

###### Breaking Input into Tokens
By default, a scanner uses white space to separate tokens. 

###### Translating Individual Tokens
The ScanXan example treats all input tokens as simple String values. Scanner also supports tokens for all of the Java language's primitive types (except for char), as well as BigInteger and BigDecimal. Also, numeric values can use thousands separators. Thus, in a US locale, Scanner correctly reads the string "32,767" as representing an integer value.






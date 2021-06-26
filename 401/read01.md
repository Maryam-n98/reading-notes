# Read: 01 - Java Basics

### Java Basics:

###### Variables:
In the Java programming language, the terms "field" and "variable" are both used.
The eight primitive data types are: byte, short, int, long, float, double, boolean, and char. The java.lang.String class represents character strings. The compiler will assign a reasonable default value for fields of the above types; for local variables, a default value is never assigned. A literal is the source code representation of a fixed value. An array is a container object that holds a fixed number of values of a single type. The length of an array is established when the array is created. After creation, its length is fixed.

###### Operators:
Simple Assignment Operator
Arithmetic Operators
Unary Operators
Equality and Relational Operators
Conditional Operators
Type Comparison Operator
Bitwise and Bit Shift Operators


###### Expressions, Statements, and Blocks:
Operators may be used in building expressions, which compute values; expressions are the core components of statements; statements may be grouped into blocks.

###### Control Flow Statements:
The statements inside your source files are generally executed from top to bottom, in the order that they appear. 


### Reddit thread on compiling:

###### Control Flow Statements
The statements inside your source files are generally executed from top to bottom, in the order that they appear. 

As you may know, everything in a computer is represented by a series of 1's and 0's (which themselves represent high and low voltages on transistors, but that's a topic for another time). When the computer runs a program, the program itself is made of a bunch of 1's and 0's.

However, since we still need humans to write our programs, putting everything in 1's and 0's (called machine language) would be very difficult. So we made higher level languages like Java and C# to write code in. These languages look a lot more like English, so they're a lot easier to write and maintain.

### Reading Java Documentation:

Java has a standard Application Programming Interface —a huge library consisting of over 4,000 classes, each with its own functionality, its own limitations, and its own rules for effective use.

To create the API documentation, the captains of Java ran a program called javadoc.
The javadoc program took lines like these right out of the PrintStream.java file and used the lines to make the documentation that you see in your web browser.

Other Java programmers do the same thing. In fact, everyone who writes Java code uses the javadoc program to generate documentation. So everyone’s Java documentation looks like everyone else’s Java documentation. When you know how read to the standard API documentation, you know how to read anybody’s homegrown Java docs.

And yes, you can use the javadoc program to create your own documentation. When you download the JDK, you get the javadoc program as part of the deal.
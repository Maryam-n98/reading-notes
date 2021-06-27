# Read: 02 - Arrays, Loops, Imports

### Packages and Import

##### Packages
In java you can  grouped the classes together in packages.
A package in Java is used to group related classes. it is as a folder in a file directory. We use packages to avoid name conflicts and to write better maintainable code.

"A package name is the same as the directory (folder) name which contains the .java files. and the The first statement, other than comments, in a Java source file, must be the package declaration. "

and there is a Default package."The project name is used as the default package name, but you can change it."
Package declaration syntax
"The statement order is as follows. Comments can go anywhere.

Package statment (optional).
Imports (optional).
Class or interface definitions."

###### Import:
 import java package into a class, we need to use java import keyword which is used to access package and its classes into the java program.

Use import to access built-in and user-defined packages into your java source file so that your class can refer to a class that is in another package by directly using its name.

And there is three options:
without import the package
import package with specified class
import package with all classes

Common imports
"There are 166 packages containing 3279 classes and interfaces in Java 5. However, only a few packages are used in most programming. GUI programs typically use at least the first three imports."

NetBeans will create your imports
"If you forgot to write import statements, or don't remember which package a class is in, no problem. Just right click on the source file and choose Fix Imports. It will add all necessary import statements."

### A Guide to Java Loops

In programming languages, loops are used to execute a set of instructions/functions repeatedly when some conditions become true. There are types of loops in Java.

Simple for loop
Enhanced for-each loop
While loop
Do-While loop


###### for loop : 
The Java for loop is a control flow statement that iterates a part of the programs multiple times.

Example	:	
for(int i=1;i<=10;i++){  
System.out.println(i);  
} 

###### While loop: 
The Java while loop is a control flow statement that executes a part of the programs repeatedly on the basis of given boolean condition.

Example: 
int i=1;  
while(i<=10){  
System.out.println(i);  
i++;  
}  

###### Do-While loop:
 The Java do while loop is a control flow statement that executes a part of the programs at least once and the further execution depends upon the given boolean condition.
Example: 
int i=1;  
do{  
System.out.println(i);  
i++;  
}



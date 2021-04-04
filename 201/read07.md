# Read07 Object-Oriented Programming, HTML Tables
## From the Domain Modeling link:
Domain Modeling

Domain modeling is the process of creating a conceptual model in code for a specific problem. A model describes the various entities, their attributes and behaviors, as well as the constraints that govern the problem domain. An entity that stores data in properties and encapsulates behaviors in methods is commonly referred to as an object-oriented model.

when you need to change the algorithm for determining popularity, the changes will be small and targeted.
Generate random numbers:
"To model the random nature of user behavior, you'll need the help of a random number generator. Fortunately, the JavaScript standard library includes a Math.random() function for just this sort of occasion."
like 

"EpicFailVideo.prototype.generateRandom = function(min, max) {
  return Math.floor(Math.random() * (max - min + 1)) + min;
}"
and its will be in object.
Math.floor, Math ceil, and Math round they fix the value of the number without percentage.
Math random: Its calculate the random the number between max and min.

The dailyLikes() method on EpicFailVideo's prototype is assigned a function with no parameters. This method starts by defining two variables called viewers and percentage.
"viewers and percentage are multiplied, rounded to the nearest integer with Math.round, and the value is returned. When the dailyLikes() method is called on both parkourFail and corgiFail, the result is logged to the console. "

## From the Duckett HTML book:
### Chapter 6: Tables
"Each block in the grid is referred to as a table cell. In HTML a table is written out row by row."
When you use an "<table>" element its written a table out row by row.
You can start each row in element "<tr>" and end it in "</tr>".
You can start each cell in element "<td>" and end it in "</td>".
"<th>" "The "<th>" element is used just like the '<td>' element but its purpose is to represent the heading for either a column or a row. (The th stands for table heading.) "
The titals of the table should put them in element "<thead>".
"The footer belongs inside the <tfoot> element."
"You can make cells of a table span more than one row or column using the rowspan and colspan attributes."

## From the Duckett JS Book:
### Chapter 3: Functions, Methods, and Objects:
To creat a new object using a comination of the keyword and the object and() then you can add properties and methods insid the object.
like var hotel = new object();
hotel.name ='park';
hotel.room =150;
and you can add some functions.
In JavaScript it will be like this:
function Hotel (name, rooms, booked) { 
this.name = name; 
this.rooms = rooms; 
this.booked = booked; 
this.checkAvailability = function() 
return this.rooms - this.booked; 
} ;
 }
 An Arrays is a special type of object its holded many of key/value pairs like the object.
 In JavaScript there are six data types: 
 1. String 2. Number 3. Boolean 4. Undefined (a variable that has been declared, but no value has been assigned to it yet) 5. Null (a variable with no value - it may have had one at some point, but no longer has a value) 6.0bject Under the hood, arrays and functions are considered types of objects. (ARRAYS ARE OBJECT).
 "Functions allow you to group a set of related statements together that represent a single task. "
 "web browsers implement objects that represent both the browser window and the document loaded into the browser window. "
"JavaScript also has several built-in objects such as String, Number, Math, and Date. Their properties and methods offer functionality that help you write scripts."
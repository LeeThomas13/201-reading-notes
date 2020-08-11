# Object-Oriented Programming, HTML Tables
<br>

## Duckett HTML Book 

<br>

### Tables (126-145)

<br>

Basic Table Structure- <table></table> = element is used to make a table. <tr></tr> = indicates the start of each row. Each cell of a table is represented using a <td></td> tag. 
<br>
EX.
<br>
<table>
  <tr>
    <th scope="col">Saturday's</th>
    <td>15</td>
    <td>16</td>
    <td>17</td>
    <td>18</td>
  </tr>
  <tr>
    <td>40</td>
    <td>45</td>
    <td>50</td>
    <td>55</td>
  </tr>
</table>
<br>
To head a table use the tag <th></th>. You can span tables and rows using the colspan attribute inside of a <th> or <td> element.
<br>
Long tables can be made by using, <thead>, <tbody>, and <tfoot> elements. (see pg.135-136)
<br>

**SUMMARY**
<br>
The <table> element is used to add tables to the web page. 
A table is drawn out row by row. Each row is created with the <tr> element.
Inside each row there are a number of cells represented by the <td> element (or <th> if it is a header)
You can make cells of a table span more than row or column using the rowspan and colspan attributes.
For long tables you can split the table into a <thead>, <tbody>, and <tfoot>.

## Duckett JS Book

<br>

### Functions, Methods, and Objects (106-144)

<br>

To update an object use dot notation or square brackets. They work on objects created using literal or constructor notation. To delete a property, use the **delete** keyword. 
<br>
EX.
<br>
hotel.name='Park';
hotel['name']='Park';
TO DELETE
delete hotel.name; or to clear the value of a property ->  hotel.name='';
<br>

**CREATING MANY OBJECTS: CONSTRUCTOR NOTATION**
<br>

Sometimes you will want several objects to represent similar things. Object constructors can use a function as a **template** for creating objects. First, create the template with the object's properties and methods.
<br>
EX.
<br>

function Hotel(name, rooms, booked) {
  this.name = name;
  this.rooms = rooms;
  this.booked = booked;

  this.checkAvailability = function() {
    return this.rooms - this.booked;
  }
}

<br>

Ways to create objects; create the object, then add properties & methods. OR create the object with properties & methods (preferred)
The Keyword *this* is referring to everything in the object and takes the name of the object. 
Arrays are actually special types of objects. They hold a related set of key value pairs, but the key for each value is its index number. There are types of built in objects. The browser object model looks like Window -> document,history,location,navigator,screen. There is a breakdown in a DOM and JS objects. See pg. 124 for browser object models.
<br>
String objects- whenever you have a value that is a string, you cna use the properties and methods of the String object on that value. This example stores the phrase "Home sweet home" in a variable.
<br>
var saying = 'Home Sweet Home '; //saying.length would give a value of 16, saying.toLowerCase would give 'home sweet home'
<br>
Math Object to create random numbers.
<br>
var randomNum = Math.floor((Math.random()) * 10) + 1);

var el = document.getElementById('info');
el.innderHTML = '<h2>random number</h2><p>' + randomNum + '</p>';
<br>

**RECAP**
<br>

1. Functions allow you to group a set of related statements together that represent a single task.
2. Functions can take parameters (information required to do their job) and may return a value.
3. An object is a series of variables and functions that represent something from the world around you.
4. In an object, variables are known as properties of the object; functions are known as methods of the object.
5. web browsers implement objects that represent both the browser window and the document loaded into the browser window.
6. Javascript also has several built-in objects such as String, Number, Math, and Date. Their properties and methods offer functionality that help you write scripts.
7. Arrays and objects can be used to create complex data sets (and both can contain the other).

## Domain Modeling (link)

<br>



[Back To Homepage](https://leethomas13.github.io/201-reading-notes/)
# Problem Domain, Objects, and the DOM

## Duckett JS Book

### Object Literals (100-105)
<br>
**What is an Object** 
<br> 
Objects group together a set of variables and functions to create a model of a something you would recognize from the real world. In an object variables become known as a *property*. In an object a function is known as a *method*. Like variables and named functions, properties and methods have a name and a value. In an object that name is called a *key*. 
<br> 
ex. 
<br> 
var hotel = {
  name: 'Quay',
  rooms: 40,
  booked: 25,
  gym: true,
  roomTypes: ['twin', 'double', 'suite'],
  checkAvailability: function() {
    return this.rooms - this.booked;
  }
}

var elName = document.getElementById('hotelName');
elName.textContent = hotel.name;

var elRooms = document.getElementById('rooms');
elRooms.textContent = hotel.checkAvalibility();
<br> 

### Document Object Model (183-242)
<br>
The DOM is a Document Object Model. It specify's how the browser should create a model of an HTML page and how JavaScript can access and update the contents of a web page while if is in the browser window. Basically the browser creates a model of all the code in one place. It can be called and manipulated. You can manipulate it by getting elements in the HTML and modifying them. When a DOM method can return moe than one element it returns a NodeList (even if it only finds one matching element).
<br>
ex.
<br>
**THE item() METHOD**
<br>
var elements = document.getElementByClassName('hot')
if (elements.length >= 1) {
  var firstItem = elements.item(0);
}
<br>
**ARRAY SYNTAX**
var elements = document.getElementByClassName('hot');
if (elements.length >= 1) {
  var firstItem = elements[0];
}
<br>
Looping through a nodelist
<br>
var hotItems = document.querySelectorAll('li.hot');         //Stores nodelist in array
if(hotItems.length > 0){    //If it contains items
  for(var i=0; i<hotItems.length; i++>) {                   //Loop through each item
    hotItems[i].className = 'cool'                          //Change value of class selectors
  } 
}



[Back To Homepage](https://leethomas13.github.io/201-reading-notes/)
# Problem Domain, Objects, and the DOM

## Duckett JS Book

### Object Literals (100-105)
&nbsp;  
**What is an Object** 
&nbsp;  
Objects group together a set of variables and functions to create a model of a something tou wold recognize from the real world. In an object variables become known as a *property*. In an object a function is known as a *method*. Like variables and named functions, properties and methods have a name and a value. In an object that name is called a *key*. 
&nbsp;  
ex. 
&nbsp;  
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
&nbsp;  




### Document Object Model (183-242)



[Back To Homepage](https://leethomas13.github.io/201-reading-notes/)
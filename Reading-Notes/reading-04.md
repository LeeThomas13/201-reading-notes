# HTML Links, CSS Layout, JS Functions

## Duckett HTML Book

### Links (74-93)

Links are created by using an <a></a> tag in your html. You specify which page you want to link to using the href attribute.
EX.
<a href="http://wwwthispagedoesntexist.com">NONEXISTANT PAGE</a>

### Layout (358-404)

Block elements are the core of layout. CSS treats each HTML element as if its in its own  box. This box will wither be a block-level box or an inline box. Block level elements start on on their own line. Inline elements flow in between surrounding text. 

CSS has positional schemes. These are normal flow, relative positioning, and absolute positioning. You can also float elements by suing the float property. In normal flow each block level element sits on top of the next element. Relative positioning moves an element in relation to where it would have been in normal flow. Absolute positioning take the box out of normal flow and no longer affects the the position of other elements on the page. Floating elements allows to yo take an element in normal flow and place it as far to the left or right of the containing element as possible.

## Duckett JS Book

### Functions, Methods, and Objects" (86-99)

declaring a function, you must name it.

EX.

function nessSmash(){
  document.write('broken')
}

you can then call the function later on. 

EX.


nessSmash()

This is helpful because once the function is declared you can utilize it later on inside of other statements. Keep in mind the variables declared within a function only exist in that function. They cannot be called upon later on. Functions can also have arguemnts. 

EX.

function getArea (width, height){
  var area  = width * height;
  return area;
}




### Article '6 Reasons of Pair Programming'

Pair programming is clearly important. It touches on all four skills: devs explain out loud what the code should do, listen to others guidance, read code that others have written, and write code themselves. It harbors greater efficiency, engages in collaboration, helps you learn from fellow students, learn social skills, helps with job interview readiness, and work enviroment readiness.


[Back To Homepage](https://leethomas13.github.io/201-reading-notes/)
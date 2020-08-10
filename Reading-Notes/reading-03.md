# HTML Lists, CSS Boxes, JS Control Flow

## Duckett HTML Book

### Lists (62-73)

-

Ordered Lists list the list items (<li></li>) the items by number. tag is <ol></ol>
-
Unordered Lists list the list items by bullet points. tag- <ul></ul>
-
Definition Lists order the list items in a 'definition sytle' by indenting. you create a 'head' to the paragraph using <dt></dt> and write under them using the <dd></dd> tag. 

Ex.

<d1>
  <dt>Ness</dt>
    <dd>Ness Is broken, his forward air is way too good, his backthrow is way too strong. Doesnt make any sense, hes a little kid. How can he throw with the force of a god.</dd>
  <dt>Smash</dt>
    <dd>Its a good game</dd>
</d1>
-
Nested Lists are useful because you can nest a list inside of a list. What a bland definition, but it works.

Ex.

<ul>
  <li>Lucina</li>
  <li>Marth</li>
  <li>Ness
    <ul>
      <li>broken</li>
      <li>good back throw</li>
      <li>dtilt is nuts</li>
    </ul>
  </li>
  <li>Captain Falcon</li>
</ul>

### Boxes (300-329)
Using CSS, you can create boxes and augment the size of them using tags like width, line-height, padding, margin, etc.
Overflow tells the browser what to do if the text within a box is larger than the box itself. You can use a hidden value or a scroll value.
Border images can be set, and their color can be set as well.
Box shadow properties allow you to drop a shadow around a box. 
Rounded corners can be utilized to round the corners of a box. these can be used by 'border-radius: 10px' '-moz-border-radius: 10px:''-webkitz-border-radius: 10px'

## Duckett JS Book

### Review: Basic Javascript Instructions (70-73)

Arrays can be used by siting a variable and assigning it an unlimited amount of values that are ordered by number. ex. var smash = [ness, lucina, marth]


### Decisions and Loops (162-182)

If Else statement checks a condition, if it resolves true the first code block is executed and if it resolves false the second code block is run.

-

Switch statements starts with a variable called the switch value. Each case indicates a possible value for this variable and the code that should run if the variable matches that value.

-

truthy values are treated as if they are true in javascript. i.e. var highScore = true; 1; 10/5; 'true'; etc.

falsy values are treated as if they are inherintly false. i.e. var highScore= false; 0; ''; ;

-

Loops come in many forms; for, while, do while. the all state a variable, a condition for that variable, and an update. i.e.
var i = 0; i<10; i++. If a loops condition is not met the loop will run again. it will run until the condition is met. Loops are very useful for counting. It can count through an array. The bigger a loop, the harder it is for the browser to load your page. 

EX.

for (var i = 0; i <10; i++)

[Back To Homepage](https://leethomas13.github.io/201-reading-notes/)




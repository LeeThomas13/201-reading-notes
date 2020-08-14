# ERROR HANDLING AND DEBUGGING

## Duckett JS Book

### Error Handling & Debugging (448-486)

JavaScript can be hard to learn, and everyone makes mistakes. This chapter will cover the console and dev tools, common problems, and handling errors.
<br>

Order of execution:
1. creates greeting variable and calls greetingUser() to get the value.
2. greetUser() returns 'hello' and the result of getName()
3. getName() returns the value 'Molly' to greetUser()
4. greetUser() returns 'Hello Molly' to the greeting variable.
5. greeting holds the value 'Hello Molly'
<br>

Functions in JS are said to have a **'Lexical Scope'** which means they are linked to the object they were defined *within*. Imagine functions as a nesting doll. The children can ask the parents for information in their variables. But the parents cannot get variables from their children. Each child will get the same answer from the parent.

<br>

ERROR OBJECTS:
1. SyntaxError- is caused by incorrect use of the rules of the language. Usually a simple typo. 
2. Reference Error- this is caused by a variable that is not declared or is out of scope.
3. Type Error- This is caused by trying to use an object or method that does not exist.
4. Range Error- of you call a function using numbers outside of its accepted range.
<br>

Console Logs can help break down your code into sections and see if its running properly.
<br>

**BREAKPOINTS**
<br>

You can pause the execution of a script on any line using breakpoints. Then you can check the values stored in variables at that point in time. in chrome; select the *sources* option. Select the script you are working with from the left-hand pane. The code will appear to the right. Find the line number you want to stop on and click on it. When you run the script, it will stop on this line. You can now hover any variable to see its value at that time in the script's execution. You can also set *conditional* breakpoints. This will only trigger that breakpoint if a condition you specify is met. The condition can use existing variables.
<br>

a debugger key can be set up to trigger breakpoints inside of JS. ex:
<br>

var $form, width, height, area;
$form = $('calculator');

$('#calculator')on('submit'. function(e) {
  e.preventDefault ();
  console.log('Clicked submit...');

  width = $('#width').val();
  height = $('#height').val();
  area = (width * height);

  if (area < 100) {
    debugger;
  }
  $form.append('<p>' +area + '</p>)
});
<br>

**SUMMARY**
1. If you understand execution contexts (which have two stages) and stacks, you are more likely to find the error in your code. 
2. Debugging is the process of finding errors. It involves a precess of deduction.
3. The console helps narrow down the area in which the error is located, so you can try to find the exact error.
4. JaavaScript has 7 different types of errors. Each creates its own error object, which can tell you its line number and gives a discription of the error.
5. If you know that you may get an error, you can handle if gracefully using the try, catch, finally statements. Use them to give your users helpful feedback.

[Back To Homepage](https://leethomas13.github.io/201-reading-notes/)


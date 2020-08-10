# Introductory HTML and JavaScript

#HTML NOTES
Attributes provide additional information about contents of an element. They appear on the opening tag of the element and are made up of two parts: a name and a value, separated by an equals sign. Opening tags can carry attributes, which tell us more about the content of that element.

Extra Markup
Utilizing ID and Class Attributes
Every element/tag can carry a unique ID or a Class. Every tag has its own unique ID that you can use to modify it. You can also assign any number of tags to a Class, making it easy to select and modify selected tags.

Block Elements
Examples are

Inline Elements
Examples are 

Grouping text and element in a block
The div element allows you to group a set of elements together in one block-level box Utilizing an ID or Class attribute on the div element can creates a CSS style rule to indicate certain changes, such as how much space the div element should occupy on the screen and change the appearance of all the elements contained with it.

Grouping text & elements inline
Using the span element acts like an inline equivalent of the div element. It is used to either contain a section of text where there is no other suitable element to differentiate it from its surrounding text.

HTML Review
article*3>img+h3+p this is how you make siblings within a parent article.

#Javascript Notes
Javascript is a way to make your website interactive and "clickable". It utilizes scripts to make things move. You set up variables and give them names, and create a functional script using logical moves. Java is housed on your browser. The browser interacts with java to make the website "clickable". However you need to imbed the java into HTML to make them merge.

Advantages of JavaScript
The merits of using JavaScript are −

Less server interaction − You can validate user input before sending the page off to the server. This saves server traffic, which means less load on your server.

Immediate feedback to the visitors − They don't have to wait for a page reload to see if they have forgotten to enter something.

Increased interactivity − You can create interfaces that react when the user hovers over them with a mouse or activates them via the keyboard.

Richer interfaces − You can use JavaScript to include such items as drag-and-drop components and sliders to give a Rich Interface to your site visitors.

Javascript Syntax
JavaScript can be implemented using JavaScript statements that are placed within the <script>... </script> HTML tags in a web page.

You can place the <script> tags, containing your JavaScript, anywhere within your web page, but it is normally recommended that you should keep it within the tags.

The <script> tag alerts the browser program to start interpreting all the text between these tags as a script. A simple syntax of your JavaScript will appear as follows.

<script ...> JavaScript code </script>
The script tag takes two important attributes −

Language − This attribute specifies what scripting language you are using. Typically, its value will be javascript. Although recent versions of HTML (and XHTML, its successor) have phased out the use of this attribute.

Type − This attribute is what is now recommended to indicate the scripting language in use and its value should be set to "text/javascript".

So your JavaScript segment will look like −

<script language = "javascript" type = "text/javascript"> JavaScript code </script>
[Back To Homepage](https://leethomas13.github.io/201-reading-notes/)
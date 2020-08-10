# HTML Text, CSS Introduction, and Basic JavaScript Instructions
CSS Notes
Stands for cascading style sheets -reads from top to bottom

header h1 { color: blue; background-color: pink

}

in this example, header and h1 is our "selector". color: blue; and background-color: pink; is called our "declaration". The entire thing is called a "ruleset".

Specificity
Box Model
- content
- padding
- border
- margin
- Its the fancy box looking thing in the dev tools on google
What we can use for colors
-rgb (red, green, blue)
-rgb(50, 250, 10)

Notes From The Book
what is CSS exactly?
     -CSS allows you to create rules that specify how the content of an element should appear. Utilizes HTML to find and work on these elements.
     
     -Rules are made up of selectors (that specify the elements the rule applies to) and declarations (that indicate what these elements should look like)
     
     -Declarations are made up of two parts: the properties of an element that you want to change, and the values of those properties.
Linking CSS to HTML
in the head of the HTML, you will see a that you plug the url/file of the CSS code

Inline Styling
you can do inline styling by adding elements in the line of code on your HTML.

Internal Styling
you can also write CSS formatted code into your html file.

Making an ID or Class
in html you are going to give certain elements ID's or Classes. you do this by typing

or and in css you access these id's by typing #nav-one {
}

or typing . for class

.nav-one {

}

Some Css tags to play with are: display, font-family, font, color, text-align, display: inline-block, float, width, height, hover.

Keep in mind you can use percentages or pixels to size things in CSS. i.e:

footer { height: 150px height: 20% }

[Back To Homepage](https://leethomas13.github.io/201-reading-notes/)
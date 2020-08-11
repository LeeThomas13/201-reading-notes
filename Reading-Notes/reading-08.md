# CSS Layout

## Duckett HTML Book

### Layout (358-404)

<br>

**THIS IS A REPEAT OF READING 04 WITH A FEW MORE DETAILS**
<br>

Block elements are the core of layout. CSS treats each HTML element as if its in its own  box. This box will wither be a block-level box or an inline box. Block level elements start on on their own line. Inline elements flow in between surrounding text. 

CSS has positional schemes. These are normal flow, relative positioning, and absolute positioning. You can also float elements by using the float property. In normal flow each block level element sits on top of the next element. Relative positioning moves an element in relation to where it would have been in normal flow. Absolute positioning take the box out of normal flow and no longer affects the the position of other elements on the page. Floating elements allows to yo take an element in normal flow and place it as far to the left or right of the containing element as possible.

*Controlling the positions of elements, creating site layouts, designing for different sized screens*
<br>

If one block-level element sits inside another block-level element then the outer box is known as the **containing** or **parent** element.
<br>

Fixed positioning is a type of absolute positioning that requires the position property to have a value of fixed. It positions the element in relation to the browser window, therefore when a user scrolls down the page it stays in the exact same place.(368)
<br>

Overlapping elements can happen when you mix absolute, relative, and fixed positioning. The elements that appear later in the  HTML code sit on **top** of the ones **earlier** in the code. (369)
<br>

Different visitors to your site will have different sized screens that show different amounts of information, so your design needs to be able to work on a range of different sized screens. Resolution refers to the ammount of dots on a screen per inch. You should shoot to keep resolution within 960-1000px since most users will be able to see this wide. Fixed and Liquid layouts (383-386)
<br>

Some devs break up their css style sheets into different files. EX. one for layout, another for fonts, another for colors, etc. Make sure you link the different style sheets in the proper place. The rules that appear in a later file will take precedent ond show up over previously stated rules.
<br>

Example Layouts (399-402)
<br>

**SUMMARY**
1. <div> elements are often used as containing elements to group together sections of a page.
2. Browsers display pages in a normal flow unless you specify relative, absolute, or fixed positioning.
3. the float property moves content to the left or right of the page and can be used to create multi-column layouts (but they require a defined width).
4. Pages can be fixed width or liquid (stretchy) layouts.
5. Designers keep pages within 960-1000px wide and indicate what the site is about within the top 600px (to demonstrate its relevance without scrolling).
6. Grids help you create professional and flexible designs.
7. CSS Framework provide rules for common tasks.
8. You can include multiple CSS files in one page.
<br>


[Back To Homepage](https://leethomas13.github.io/201-reading-notes/)
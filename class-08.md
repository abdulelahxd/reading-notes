**Key Concepts in Positioning El ements** 

Building Blocks
CSS treats each HTML element as if it is in its
own box. This box will either be a block-level
box or an inline box.
Block-level boxes start on a new line and act as the main building blocks
of any layout, while inline boxes flow between surrounding text. You can
control how much space each box takes up by setting the width of the
boxes (and sometimes the height, too). To separate boxes, you can use
borders, margins, padding, and background colors.  

![](https://www.pluralsight.com/content/pluralsight/en/blog/film-games/und/understand-inline-and-block-level-elements/_jcr_content/main/hero_blog_block/image-res.img.jpg/1501612380025.jpg)

Block-level elements
start on a new line
Examples include:
```<h1> <p> <ul> <li>```


Inline elements
flow in between
surrounding text
Examples include:
```<img> <b> <i>```





**Controll ing the Position of El ements**

1. Normal flow
Every block-level element
appears on a new line, causing
each item to appear lower down
the page than the previous one.
Even if you specify the width
of the boxes and there is space
for two elements to sit side-byside,
they will not appear next
to each other. This is the default
behavior (unless you tell the
browser to do something else).

2. Relative Positioning
This moves an element from the
position it would be in normal
flow, shifting it to the top, right,
bottom, or left of where it
would have been placed. This
does not affect the position of
surrounding elements; they stay
in the position they would be in
in normal flow.

3. This positions the element
in relation to its containing
element. It is taken out of
normal flow, meaning that it
does not affect the position
of any surrounding elements
(as they simply ignore the
space it would have taken up).
Absolutely positioned elements
move as users scroll up and
down the page.


4. Fixed Positioning
This is a form of absolute
positioning that positions
the element in relation to the
browser window, as opposed
to the containing element.
Elements with fixed positioning
do not affect the position of
surrounding elements and they
do not move when the user
scrolls up or down the page.

5. Floating Elements
Floating an element allows
you to take that element out
of normal flow and position
it to the far left or right of a
containing box. The floated
element becomes a block-level
element around which other
content can flow.



# Screen Resolution

>## Resolution refers to the number of dots a screen shows per inch. Some devices have a higher resolution than desktop computers and most operating systems allow users to adjust the resolution of their screens.


# Page Sizes 

>## Because screen sizes and display resolutions vary so much, web designers often try to create pages of around 960-1000 pixels wide (since most users will be able to see designs this wide on their screens).




# CSS Frameworks

CSS frameworks aim to make your life easier by providing the code for
common tasks, such as creating layout grids, styling forms, creating
printer-friendly versions of pages and so on. You can include the CSS
framework code in your projects rather than writing the CSS from scratch.




# Multiple Style Sheets
1. ```@import```

>Some web page authors split
up their CSS style rules into
separate style sheets. For
example, they might use one
style sheet to control the layout
and another to control fonts,
colors and so on.
Some authors take an even
more modular approach
to stylesheets, creating
separate stylesheets to control
typography, layout, forms,
tables, even different styles for
each sub-section of a site.
There are two ways to add
multiple style sheets to a page:
1: Your HTML page can link
to one style sheet and that
stylesheet can use the @import
rule to import other style sheets.
2: In the HTML you can use a
separate ```<link> ```element for
each style sheet.


2. ```link```
On this page you can see the
other technique for including
multiple style sheets. Inside the
```<head> ```element is a separate
```<link>``` element for each style
sheet.
The contents of site.css are
identical to styles.css on the
left hand page, except the code
does not contain @import rules.
As with all style sheets, if two
rules apply to the same element
then rules that appear later in a
document will take precedence
over previous rules.


```
1. <div> elements are often used as containing elements to group together sections of a page.
2.  Browsers display pages in normal flow unless you specify relative, absolute, or fixed positioning.
3. The float property moves content to the left or right of the page and can be used to create multi-column layouts. (Floated items require a defined width.)
4. Pages can be fixed width or liquid (stretchy) layouts.
5. Designers keep pages within 960-1000 pixels wide, and indicate what the site is about within the top 600 pixels (to demonstrate its relevance without scrolling).
6. Grids help create professional and flexible designs.
7. CSS Frameworks provide rules for common tasks.
8. You can include multiple CSS files in one page.
```
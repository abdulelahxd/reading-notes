# HTML TEXT FORMAtTING

![pic](https://www.templatemonster.com/blog/wp-content/uploads/2018/12/overapi.jpg)

there are many tags to format text as you like in **HTML** to make it clearer and more understandable and organized.

HTML elements are used to describe the structure of
the page (e.g. headings, subheadings, paragraphs).

They also provide semantic information (e.g. where
emphasis should be placed, the definition of any
acronyms used, when given text is a quotation).

# CSS 

## CSS works by associating rules with HTML elements. These rules govern how the content of specified elements should be displayed. A CSS rule contains two parts: a selector and a declaration.

1. This rule indicates that all <p>
elements should be shown in the
Arial typeface.

2. Selectors indicate which
element the rule applies to.
The same rule can apply to
more than one element if you
separate the element names
with commas.


3. Declarations indicate how
the elements referred to in
the selector should be styled.
Declarations are split into two
parts (a property and a value),
and are separated by a colon.

## CSS declarations sit inside curly brackets and each is made up of two parts: a property and a value, separated by a colon. You can specify several properties in one declaration, each separated by a semi-colon.

1. Properties indicate the aspects
of the element you want to
change. For example, color, font,
width, height and border.

2. Values specify the settings
you want to use for the chosen
properties. For example, if you
want to specify a color property
then the value is the color you
want the text in these elements
to be.



When building a website there are several advantages to placing your
CSS rules in a separate style sheet.

1. All of your web pages can share
the same style sheet. This is
achieved by using the ```<link>```
element on each HTML page of
your site to link to the same CSS
document. This means that the
same code does not need to be
repeated in every page (which
results in less code and smaller
HTML pages).

2. Therefore, once the user has
downloaded the CSS stylesheet,
the rest of the site will load
faster. If you want to make a
change to how your site appears,
you only need to edit the one
CSS file and all of your pages
will be updated. For example,
you can change the style of
every``` <h1>``` element by altering

3. the one CSS style sheet, rather
than changing the CSS rules on
every page. The HTML code
will be easier to read and edit
because it does not have lots of
CSS rules in the same document.
It is generally considered good
practice to have the content of
the site separated from the rules
that determine how it appears.


1. CSS treats each HTML e  lement as if it appears inside
its own box and uses rules to indicate how that
element should look.

2. Rules are made up of selectors (that specify the
elements the rule applies to) and declarations (that
indicate what these elements should look like).

3. Different types of selectors allow you to target your
rules at different elements.

4. Declarations are made up of two parts: the properties
of the element that you want to change, and the values
of those properties. For example, the font-family
property sets the choice of font, and the value arial
specifies Arial as the preferred typeface.

5. CSS rules usually appear in a separate document,
although they may appear within an HTML page.



# JavaScript 

A script is a series of instructions that a computer can follow one-by-one.
Each individual instruction or step is known as a statement.
Statements should end with a semicolon.

You should write comments to explain what your code does.
They help make your code easier to read and understand.
This can help you and others who read your code. 

1. MULTI-LINE COMMENTS
To write a comment that stretches over more than
one line, you use a multi-line comment, starting with
the /* characters and ending with the * / characters.
Anything between these characters is not processed·
by the JavaScript interpreter.

2. SINGLE-LINE COMMENTS
In a single-line comment, anything that follows the
two forward slash characters I/ on that line will not
be processed by the JavaScript interpreter. Singleline
comments are often used for short descriptions
of what the code is doing.

 *JavaScript distinguishes between numbers strings, and true or false values known as Booleans.*


## An array is a special type of variable. It doesn't just store one value; it stores a list of values.

``` var colors = new Array( 'white ' ,  ```
                           ``` 'black', ```
                          ```  'custom ' ); ```



Values in an array are accessed as if they are in
a numbered list. It is important to know that the
numbering of this list starts at zero (not one).

NUMBERING ITEMS IN
AN ARRAY
Each item in an array is
automatically given a number
called an index. This can be used
to access specific items in the
array. Consider the following
array which holds three colors:
var col ors;
colors= ['whi te ' ,
'black ' ,
' custom'];
Confusingly, index values start at
0 (not 1), so the following table
shows items from the array and
their corresponding index values:
INDEX VALUE
o 'white '
'bl ack'
2 ' custom'


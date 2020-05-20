# Forms 

The best known form on the web is probably
the search box that sits right in the middle of
Google's homepage.  

Form Controls  
There are several types of form controls that
you can use to collect information from visitors
to your site. 




1. ADDING TEXT

2.  Making Choices

3.  Submitting Forms

4.  Uploading Files

>```<form>```
Form controls live inside a
```<form> ```element. This element
should always carry the action
attribute and will usually have a
method and id attribute too.

  
1. action Every ```<form>``` element requires an action attribute. Its value is the URL for the page on the server that will receive the information in the form when it is submitted.

2. method Forms can be sent using one of two methods: get or post.
With the get method, the values from the form are added to the end of the URL specified in the action attribute. The get method is ideal for:
short forms (such as search boxes)  when you are just retrieving data from the web server (not sending information that should be added to or deleted from a database)
3.``` <input> ```The ```<input> ```element is used to create several different form
controls. The value of the type attribute determines what kind of input they will be creating.
4. type="text" When the type attribute has a
value of text, it creates a singleline
text input.
5. name When users enter information into a form, the server needs to know which form control each piece of data was entered into. (For example, in a login form, the
server needs to know what has been entered as the username
and what has been given as the password.) Therefore, each form
control requires a name attribute. The value of this attribute
identifies the form control and is sent along with the information
they enter to the server.
6.  maxlength You can use the maxlength attribute to limit the number
of characters a user may enter into the text field. Its value is the
number of characters they may enter. For example, if you were
asking for a year, the maxlength attribute could have a value of 4.

# Table
width to set the width of the
table
padding to set the space
between the border of each table
cell and its content
text-transform to convert the
content of the table headers to
uppercase
letter-spacing, font-size
to add additional styling to the
content of the table headers
border-top, border-bottom
to set borders above and below
the table headers
text-align to align the writing
to the left of some table cells and
to the right of the others
background-color to change
the background color of the
alternating table rows
:hover to highlight a table row
when a user's mouse goes over it 

>In addition to the CSS p  roperties covered in other
chapters which work with the contents of all elements,
there are several others that are specifically used to
control the appearance of lists, tables, and forms.  

> List markers can be given different appearances
using the list-style-type and list-style image
properties.


> Table cells can have different borders and spacing in
different browsers, but there are properties you can
use to control them and make them more consistent.


> Forms are easier to use if the form controls are
vertically aligned using CSS.

> Forms benefit from styles that make them feel more
interactive.




# Events 
HOW EVENTS TRIGGER
JAVASCRIPT CODE 

When the user interacts with the HTML on a web page, there are three
steps involved in getting it to trigger some JavaScript code.
Together these steps are known as event handling.


1.  Select t he element
node(s) you want the
script to respond to.
For example, if you want to
trigger a function when a user
clicks on a specific link, you need
to get the DOM node for that
link element. You do this using a
DOM query (see Chapter 5).

2. Indicate which event on
the selected node(s) will
trigger the response.
Programmers call this binding an
event to a DOM node.
The previous two pages showed
a selection of the popular events
that you can monitor for.
3. State the code you want
to run when the event
occurs.
When the event occurs, on a
specified element, it will trigger
a function. This may be a named
or an anonymous function.




When an event occurs, the event object tells
you information about the event, and the
element it happened upon 

Every time an event fires, the The event object is passed to
event object contains helpful any function that is the event
data about the event, such as: handler or listener.
• Which element the event
happened on If you need to pass arguments
• Which key was pressed for a to a named function, the event
keypress event object will first be passed to the
• What part of the viewport the anonymous wrapper function
user clicked for a c 1 i ck event (this happens automatically);
(the viewport is the part of then you must specify it as a
the browser window that parameter of the named function
shows the web page) (as shown on the next page).
When the event object is
passed into a function, it is often
given the parameter name e
(for event). It is a widely used
shorthand (and you see it
adopted throughout this book).
Note, however, that some
programmers also use the
parameter name e to refer to the
error object; so e may mean
event or error in some scripts.

1. Events are the browser's way of indicating when
something has happened (such as when a page has
finished loading or a button has been clicked).
2. Binding is the process of stating which event you are
waiting to happen, and which element you are waiting
for that event to happen upon.
3. When an event occurs on an element, it can trigger a
JavaScript function. When this function then changes
the web page in some way, it feels interactive because
it has responded to the user.
4. You can use event delegation to monitor for events
that happen on all of the children of an element.
5. The most commonly used events are W3C DOM
events, although there are others in the HTMLS
specification as well as browser-specific events.
## WHAT IS AN OBJECT

Objects group together a set of variables and functions to create a model
of a something you would recognize from the real world. In an object,
variables and functions take on new names.

![js](https://cdn-media-1.freecodecamp.org/images/1*5dbaz5S1Buevb-fZQDbYzg.jpeg)

IN AN OBJECT: VARIABLES BECOME
KNOWN AS PROPERTIES
If a variable is part of an object, it is called a
property. Properties te ll us about the object


IN AN OBJECT: FUNCTIONS BECOME
KNOWN AS METHODS
If a function is part of an object, it is called a method.
Methods represent tasks that are associated with
the object.


**The Document Object Model (DOM) specifies how browsers should create a model of an HTML page and how JavaScript can access and update the contents of a web page while it is in the browser window.**



![jjs](https://2r4s9p1yi1fa2jd7j43zph8r-wpengine.netdna-ssl.com/files/2017/09/assembling-2.png)

1. getElementByld( 1 id 1) Selects an individual element given the value of its i d attribute . The HTML must have an id attribute in order for it to be selectable.

2. querySel ector( 1css selector ') Uses CSS selector syntax that would select one or more elements. This method returns only the first of the matching elements.


3. getEl ement sByClassName( 1class 1) Selects one or more elements given the va lue of their cl ass attribute.
The HTML must have a cl ass attribu te for it to be selectable.
This method is faster than querySe 1ectorA11 ().



4. getEl ementsByTagName( 1 tagName 1)
Selects all elements on the page with the specified tag name.
This method is faster than querySe 1ectorA11 ().


5. querySelectorAll ( 1css select or •)
Uses CSS selector syntax to select one or more elements and returns all
of those that match.




>REMOVING ELEMENTS VIA
DOM MANIPULATION 

DOM manipulation can be used to remove
elements from the DOM tree. 
1. STORE THE ELEMENT
TO BE REMOVED IN A
VARIABLE
You start by selecting the
element that is going to be
removed and store that element
node in a variable.
You can use any of the methods
you saw in the section on DOM
queries to select the element.

2. STORE THE PARENT OF
THAT ELEMENT IN A
VARIABLE
Next, you find the parent element
that contains the element you
want to remove and store that
element node in a variable.
The simplest way to get this
element is to use the parentNode
property of this element.

3. REMOVE THE ELEMENT
FROM ITS CONTA INING
ELEMENT
The removeChi ld() method is
used on the containing element
that you selected in step 2.
The removeChi ld() method
takes one parameter: the
reference to the element that
you no longer want.

  
> 1. The browser represents the page using a DOM tree.
> 2. DOM trees have four types of nodes: document nodes,
>element nodes, attribute nodes, and text nodes.
> 3. You can select element nodes by their id or cl ass
>attributes, by tag name, or using CSS selector syntax.
> 4. Whenever a DOM query can return more than one
>node, it will always return a Nadel i st.
> 5. From an element node, you can access and update its
>content using properties such as textContent and
>i nnerHTML or using DOM manipulation techniques.
> 6. An element node can contain multiple text nodes and
>child elements that are siblings of each other.
>7. In older browsers, implementation of the DOM is
>inconsistent (and is a popular reason for using jQuery).
> 8. Browsers offer tools for viewing the DOM tree .




















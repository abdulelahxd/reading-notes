# What's a Table?
A table represents information in a grid format.
Examples of tables include financial reports, TV
schedules, and sports results.

Basic Table St ructure


![s](https://magenic.com/media/2345/tables2.png)

``` 
<table>
The <table> element is used
to create a table. The contents
of the table are written out row
by row.


<tr>
You indicate the start of each
row using the opening <tr> tag.
(The tr stands for table row.)
It is followed by one or more
<td> elements (one for each cell
in that row).
At the end of the row you use a
closing </tr> tag.


<td>
Each cell of a table is
represented using a <td>
element. (The td stands for
table data.)
At the end of each cell you use a
closing </td> tag. 


<th>
The <th> element is used just
like the <td> element but its
purpose is to represent the
heading for either a column or
a row. (The th stands for table
heading.)
Even if a cell has no content,
you should still use a <td> or
<th> element to represent
the presence of an empty cell
otherwise the table will not
render correctly. (The first cell
in the first row of this example
shows an empty cell.)
```

The ```<table>``` element is used to add tables to a web
page.
 A table is drawn out row by row. Each row is created
with the ```<tr> ```element.
 Inside each row there are a number of cells
represented by the``` <td> ```element (or``` <th>``` if it is a
header).
 You can make cells of a table span more than one row
or column using the rowspan and colspan attributes.
 For long tables you can split the table into a``` <thead>,```
```<tbody>,``` and``` <tfoot>.```    









# What is the DOM?
The Document Object Model (DOM) is a programming interface for HTML and XML documents. It represents the page so that programs can change the document structure, style, and content. The DOM represents the document as nodes and objects. That way, programming languages can connect to the page.

![s2](https://cdn-media-1.freecodecamp.org/images/1*5dbaz5S1Buevb-fZQDbYzg.jpeg)


## object 
1. BROWSER OBJECT MODEL  
The Browser Object Model contains
objects that represent the current
browser window or tab. It contains
objects that model things like
browser history and the
device's screen.

2. DOCUMENT OBJECT MODEL  
The Document Object Model uses
objects to create a representation of
the current page. It creates a new
object for each element (and each
individual section of text)
within the page.

3. GLOBAL JAVASCRIPT OBJECTS  
The global JavaScript objects
represent things that the JavaScript
language needs to create a model
of. For example, there is an
object that deals only with
dates and times.


# Python Scope

*The scope of a name or variable depends on the place in your code where you create that variable. The Python scope concept is generally presented using a rule known as the LEGB rule.*

>The letters in the acronym LEGB stand for Local, Enclosing, Global, and Built-in scopes.

<hr>

the scope of a name defines the area of a program in which you can unambiguously access that name, such as variables, functions, objects, and so on. A name will only be visible to and accessible by the code in its scope. Several programming languages take advantage of scope for avoiding name collisions and unpredictable behaviors. Most commonly, you’ll distinguish two general scopes:

* **Global scope**: The names that you define in this scope are available to all your code.

* **Local scope**: The names that you define in this scope are only available or visible to the code within the scope.


## The Global Scope
*From the moment we start a Python program, we are in the global Python scope. Internally, Python turns our program’s main script into a module called ``` __main__ ```to hold the main program’s execution. The namespace of this module is the main global scope of your program.*

>Note: In Python, the notions of global scope and global names are tightly associated with module files. For example, if you define a name at the top level of any Python module, then that name is considered global to the module. That’s the reason why this kind of scope is also called module scope.

<hr>

## The nonlocal Statement

*Similarly to global names, nonlocal names can be accessed from inner functions, but not assigned or updated. If you want to modify them, then you need to use a nonlocal statement. With a nonlocal statement, you can define a list of names that are going to be treated as nonlocal.*

The nonlocal statement consists of the nonlocal keyword followed by one or more names separated by commas. These names will refer to the same names in the enclosing Python scope. The following example shows how you can use nonlocal to modify a variable defined in the enclosing or nonlocal scope: 

EX 
```
>>> def func():
...     var = 100  # A nonlocal variable
...     def nested():
...         nonlocal var  # Declare var as nonlocal
...         var += 100
...
...     nested()
...     print(var)
...
>>> func()
200
```

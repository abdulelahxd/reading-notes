# FileIO & Exceptions

## What Is a File in python?
a file is a contiguous set of bytes used to store data. This data is organized in a specific format and can be anything as simple as a text file or as complicated as a program executable. In the end, these byte files are then translated into binary 1 and 0 for easier processing by the computer.

* Header: metadata about the contents of the file (file name, size, type, and so on)

* Data: contents of the file as written by the creator or editor

* End of file (EOF): special character that indicates the end of the file

<hr>

## Opening and Closing a File in Python

### opening
When you want to work with a file, the first thing to do is to open it. This is done by invoking the open() built-in function. open() has a single required argument that is the path to the file. open() has a single return: 

Ex 
```
file = open('dog_breeds.txt')
```
>Warning: You should always make sure that an open file is properly closed.

### closing
t’s important to remember that it’s your responsibility to close the file. In most cases, upon termination of an application or script, a file will be closed eventually. However, there is no guarantee when exactly that will happen. This can lead to unwanted behavior including resource leaks. It’s also a best practice within Python (Pythonic) to make sure that your code behaves in a way that is well defined and reduces any unwanted behavior.

When you’re manipulating a file, there are two ways that you can use to ensure that a file is closed properly, even when encountering an error. The first way to close a file is to use the try-finally block:

Ex 
```
reader = open('dog_breeds.txt')
try:
    # Further file processing goes here
finally:
    reader.close()
```

The second way to close a file is to use the with statement:

Ex 
```
with open('dog_breeds.txt') as reader:
    # Further file processing goes here
```
<hr>

## Reading and Writing Opened Files

Method  |  What It Does
--------- | ---------
.read(size=-1) | This reads from the file based on the number of size bytes. If no argument is passed or None or -1 is passed, then the entire file is read.
.readline(size=-1) |  This reads at most size number of characters from the line. This continues to the end of the line and then wraps back around. If no argument is passed or None or -1 is passed, then the entire line (or rest of the line) is read.
.readlines() | 	This reads the remaining lines from the file object and returns them as a list.

<br>

EX 
```
with open('dog_breeds.txt', 'r') as reader:
    # Read & print the entire file
    print(reader.read())
Pug
Jack Russell Terrier
English Springer Spaniel
German Shepherd
Staffordshire Bull Terrier
Cavalier King Charles Spaniel
Golden Retriever
West Highland White Terrier
Boxer
Border Terrier
```
writing files. As with reading files, file objects have multiple methods that are useful for writing to a file:
Method  |  What It Does
--------- | ---------
.write(string) | 	This writes the string to the file.
.writelines(seq) | This writes the sequence to the file. No line endings are appended to each sequence item. It’s up to you to add the appropriate line ending(s).

EX 
```
with open('dog_breeds.txt', 'r') as reader:
    # Note: readlines doesn't trim the line endings
    dog_breeds = reader.readlines()

with open('dog_breeds_reversed.txt', 'w') as writer:
    # Alternatively you could use
    # writer.writelines(reversed(dog_breeds))

    # Write the dog breeds to the file in reversed order
    for breed in reversed(dog_breeds):
        writer.write(breed)
```

# Exceptions versus Syntax Errors

## Raising an Exception it's like a way to make sure that our specific code block is working fine like if we got nothing from raise expection then we are good to go to the second block. as well as the assert thing will make sure about the block is executed as it should.

```
TRY EXPECT ELSE 

In Python, using the else statement, you can instruct a program to execute a certain block of code only in the absence of exceptions.
```


* raise allows you to throw an exception at any time.
* assert enables you to verify if a certain condition is met and throw an exception if it isn’t.
* In the try clause, all statements are executed until an exception is encountered.
* except is used to catch and handle the exception(s) that are encountered in the try clause.
* else lets you code sections that should run only when no exceptions are encountered in the try clause.
* finally enables you to execute sections of code that should always run, with or without any previously encountered exceptions.
# AirBnB clone

The goal of this project is to deploy a simple copy of the [AirBnB website](https://www.airbnb.com/).  
However, not all features are implemented, only some just to cover fundamental development concepts.  
The project includes:

* A console to manipulate data without a visual interface
* A website(the front-end) that shows the final product: Static and Dynamic
* A database/files that stores data
* An API that provides a communication interface between the frontend and the backend

## Directory structure


## The console

The first piece is to manipulate a powerful storage system.  
This storage engine gives an abstraction between objects and how they are stored and persisted.  
This means, from the console, the front-end and RestAPI, you don't have to take care of how objects are stored.  
This abstraction also allows you to change the type of storage easily without updating the entire codebase.  
The console is the tool used to validate the storage engine.  

![Console](/screenshots/console.png)

The console is able to:
* Create a new object (ex: a new User or a new Place)
* Retrieve an object from a file or a database
* Do operations on objects(count, compute stats)
* Update attributes of an object
* Destroy an object

### Getting started with the console

To see how the console works, clone this repo on your local machine.  
The console's entry point should be the file `console.py`.  
To start the console, ensure the file has executable rights and run `./console.py` in the same directory.    
The console works in both interactive and non-interactive modes.  

```sh

# Interactive mode

$ ./console.py
(hbnb) help

Documented commands (type help <topic>):
========================================
EOF  help  quit

(hbnb) 
(hbnb) 
(hbnb) quit
$

```


```sh

$ echo "help" | ./console.py
(hbnb)

Documented commands (type help <topic>):
========================================
EOF  help  quit
(hbnb)
$
$ cat test_help
help
$
$ cat test_help | ./console.py
(hbnb)

Documented commands (type help <topic>):
========================================
EOF  help  quit
(hbnb)
$

```

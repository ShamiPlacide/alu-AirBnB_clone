# AirBnB Clone Project

This project is part of the **ALU Software Engineering curriculum**. It is the first step towards building a full web application that mimics the core functionality of [AirBnB](https://www.airbnb.com).

## Project Overview
The initial phase focuses on creating a **command-line interpreter** to manage AirBnB objects.  
This interpreter serves as a foundation for validating the storage engine and future development stages.

## Command Interpreter

### How to Start It

#### Interactive Mode
```bash
$ ./console.py
(hbnb) help

Documented commands (type help ):
EOF  help  quit
(hbnb)
(hbnb) quit
$
#### Non-Interactive Mode
$ echo "help" | ./console.py
(hbnb)
Documented commands (type help ):
EOF  help  quit
(hbnb)
$
#### How to Use It

The command interpreter supports the following commands:

create – Creates a new instance of a class.

show – Prints the string representation of an instance.

destroy – Deletes an instance based on the class name and id.

all – Prints all string representations of all instances.

update – Updates an instance based on the class name and id.

#### Examples
$ ./console.py
(hbnb) create BaseModel
49faff9a-6318-451f-87b6-910505c55907

(hbnb) all BaseModel
["[BaseModel] (49faff9a-6318-451f-87b6-910505c55907) {'created_at': datetime.datetime(2022, 10, 28, 21, 3, 54, 52298), 'id': '49faff9a-6318-451f-87b6-910505c55907', 'updated_at': datetime.datetime(2022, 10, 28, 21, 3, 54, 52302)}"]

(hbnb) show BaseModel 49faff9a-6318-451f-87b6-910505c55907
[BaseModel] (49faff9a-6318-451f-87b6-910505c55907) {'created_at': datetime.datetime(2022, 10, 28, 21, 3, 54, 52298), 'id': '49faff9a-6318-451f-87b6-910505c55907', 'updated_at': datetime.datetime(2022, 10, 28, 21, 3, 54, 52302)}

(hbnb) destroy BaseModel 49faff9a-6318-451f-87b6-910505c55907
(hbnb) show BaseModel 49faff9a-6318-451f-87b6-910505c55907
** no instance found **

(hbnb) quit
$
## Project Features

Command-line interface for object management.

Supports CRUD operations (create, show, destroy, all, update).

Data persistence via a storage engine.

Modular design to allow future development into a web application.

Directory Structure

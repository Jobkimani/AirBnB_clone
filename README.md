# AirBnB Clone Console

## Table of Contents

* [Introduction](#introduction)
* [Environment](#environment)
* [Installation](#installation)
* [Testing](#testing)
* [Usage](#usage)
* [Authors](#authors)

## Introduction

This is a team project aimed at building a clone of [AirBnB](https://www.airbnb.com/). The console serves as a command interpreter for managing object abstractions and their storage.

For a deeper understanding of the project, refer to the [Wiki](https://github.com/ralexrivero/AirBnB_clone/wiki).

The console performs the following tasks:

* Create a new object
* Retrieve an object from a file
* Perform operations on objects
* Destroy an object

### Storage

All classes are handled by the `Storage` engine in the `FileStorage` class.

## Environment

* Ubuntu: [![Ubuntu](https://img.shields.io/static/v1?label=&message=Ubuntu&color=E95420&logo=Ubuntu&logoColor=E95420&labelColor=2F333A)](https://ubuntu.com/)
* Bash: [![Bash](https://img.shields.io/static/v1?label=&message=GNU%20Bash&color=4EAA25&logo=GNU%20Bash&logoColor=4EAA25&labelColor=2F333A)](https://www.gnu.org/software/bash/)
* Python: [![Python](https://img.shields.io/static/v1?label=&message=Python&color=FFD43B&logo=python&logoColor=3776AB&labelColor=2F333A)](https://www.python.org/)
* Vim: [![Vim](https://img.shields.io/static/v1?label=&message=Vim&color=019733&logo=Vim&logoColor=019733&labelColor=2F333A)](https://www.vim.org/)
* VS Code: [![VS Code](https://img.shields.io/static/v1?label=&message=Visual%20Studio%20Code&color=5C2D91&logo=Visual%20Studio%20Code&logoColor=5C2D91&labelColor=2F333A)](https://code.visualstudio.com/)
* Git: [![Git](https://img.shields.io/static/v1?label=&message=Git&color=F05032&logo=Git&logoColor=F05032&labelColor=2F333A)](https://git-scm.com/)
* GitHub: [![GitHub](https://img.shields.io/static/v1?label=&message=GitHub&color=181717&logo=GitHub&logoColor=f2f2f2&labelColor=2F333A)](https://github.com)

### Style Guidelines

* [pycodestyle (version 2.7.*)](https://pypi.org/project/pycodestyle/)
* [PEP8](https://pep8.org/)

Development and testing were conducted on Ubuntu 20.04 LTS using Python 3.8.3. Editors included VIM 8.1.2269, VSCode 1.6.1, and Atom 1.58.0. Version control utilized Git 2.25.1.

## Installation

```bash
git clone https://github.com/aysuarex/AirBnB_clone.git
cd AirBnb
./console.py



Execution
Interactive Mode:




$ ./console.py
(hbnb) help

Documented commands (type help <topic>):
========================================
EOF  help  quit

(hbnb)
(hbnb)
(hbnb) quit
$



Non-interactive Mode:



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



Testing
All tests are defined in the tests folder.

Documentation
Modules:



python3 -c 'print(__import__("my_module").__doc__)'



Classes:


python3 -c 'print(__import__("my_module").MyClass.__doc__)'




Functions (inside and outside a class):

python3 -c 'print(__import__("my_module").my_function.__doc__)'



python3 -c 'print(__import__("my_module").MyClass.my_function.__doc__)'




Python Unit Tests
unittest module
File extension .py
Files and folders start with test_
Organization: for models/base.py, unit tests in: tests/test_models/test_base.py
Execution command: python3 -m unittest discover tests
or: python3 -m unittest tests/test_models/test_base.py
Run Test in Interactive Mode:

echo "python3 -m unittest discover tests" | bash



Run Test in Non-interactive Mode:


python3 -m unittest discover tests



Usage
Start the console in interactive mode:



$ ./console.py
(hbnb)

Use help to see the available commands:

(hbnb) help

Documented commands (type help <topic>):
========================================
EOF  all  count  create  destroy  help  quit  show  update

(hbnb)


Quit the console:

(hbnb) quit
$



(hbnb) quit
$


create <class>

(hbnb) create BaseModel
6cfb47c4-a434-4da7-ac03-2122624c3762
(hbnb)

show <class> <id>
(hbnb) show BaseModel 6cfb47c4-a434-4da7-ac03-2122624c3762
[BaseModel] (a) [BaseModel] (6cfb47c4-a434-4da7-ac03-2122624c3762) {'id': '6cfb47c4-a434-4da7-ac03-2122624c3762', 'created_at': datetime.datetime(2021, 11, 14, 3, 28, 45, 571360), 'updated_at': datetime.datetime(2021, 11, 14, 3, 28, 45, 571389)}
(hbnb)




Destroy:

(hbnb) create User
0c98d2b8-7ffa-42b7-8009-d9d54b69a472
(hbnb) destroy User 0c98d2b8-7ffa-42b7-8009-d9d54b69a472
(hbnb) show User 0c98d2b8-7ffa-42b7-8009-d9d54b69a472
** no instance found **
(hbnb)


All
(hbnb) create BaseModel
e45ddda9-eb80-4858-99a9-226d4f08a629
(hbnb) all BaseModel
["[BaseModel] (4c8f7ebc-257f-4ed1-b26b-e7aace459897) [BaseModel] (4c8f7ebc-257f-4ed1-b26b-e7aace459897) {'id': '4c8f7ebc-257f-4ed1-b26b-e7aace459897', 'created_at': datetime.datetime(2021, 11, 13, 22, 19, 19, 447155), 'updated_at': datetime.datetime(2021, 11, 13, 22, 19, 19, 447257), 'name': 'My First Model', 'my_number': 89}"]
...


markdown
Copy code
# AirBnB Clone Console

## Table of Contents

* [Introduction](#introduction)
* [Environment](#environment)
* [Installation](#installation)
* [Testing](#testing)
* [Usage](#usage)
* [Authors](#authors)

## Introduction

This is a team project aimed at building a clone of [AirBnB](https://www.airbnb.com/). The console serves as a command interpreter for managing object abstractions and their storage.

For a deeper understanding of the project, refer to the [Wiki](https://github.com/ralexrivero/AirBnB_clone/wiki).

The console performs the following tasks:

* Create a new object
* Retrieve an object from a file
* Perform operations on objects
* Destroy an object

### Storage

All classes are handled by the `Storage` engine in the `FileStorage` class.

## Environment

* Ubuntu: [![Ubuntu](https://img.shields.io/static/v1?label=&message=Ubuntu&color=E95420&logo=Ubuntu&logoColor=E95420&labelColor=2F333A)](https://ubuntu.com/)
* Bash: [![Bash](https://img.shields.io/static/v1?label=&message=GNU%20Bash&color=4EAA25&logo=GNU%20Bash&logoColor=4EAA25&labelColor=2F333A)](https://www.gnu.org/software/bash/)
* Python: [![Python](https://img.shields.io/static/v1?label=&message=Python&color=FFD43B&logo=python&logoColor=3776AB&labelColor=2F333A)](https://www.python.org/)
* Vim: [![Vim](https://img.shields.io/static/v1?label=&message=Vim&color=019733&logo=Vim&logoColor=019733&labelColor=2F333A)](https://www.vim.org/)
* VS Code: [![VS Code](https://img.shields.io/static/v1?label=&message=Visual%20Studio%20Code&color=5C2D91&logo=Visual%20Studio%20Code&logoColor=5C2D91&labelColor=2F333A)](https://code.visualstudio.com/)
* Git: [![Git](https://img.shields.io/static/v1?label=&message=Git&color=F05032&logo=Git&logoColor=F05032&labelColor=2F333A)](https://git-scm.com/)
* GitHub: [![GitHub](https://img.shields.io/static/v1?label=&message=GitHub&color=181717&logo=GitHub&logoColor=f2f2f2&labelColor=2F333A)](https://github.com)

### Style Guidelines

* [pycodestyle (version 2.7.*)](https://pypi.org/project/pycodestyle/)
* [PEP8](https://pep8.org/)

Development and testing were conducted on Ubuntu 20.04 LTS using Python 3.8.3. Editors included VIM 8.1.2269, VSCode 1.6.1, and Atom 1.58.0. Version control utilized Git 2.25.1.

## Installation

```bash
git clone https://github.com/aysuarex/AirBnB_clone.git
cd AirBnb
./console.py
Execution
Interactive Mode:

bash
Copy code
$ ./console.py
(hbnb) help

Documented commands (type help <topic>):
========================================
EOF  help  quit

(hbnb)
(hbnb)
(hbnb) quit
$
Non-interactive Mode:

bash
Copy code
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
Testing
All tests are defined in the tests folder.

Documentation
Modules:
python
Copy code
python3 -c 'print(__import__("my_module").__doc__)'
Classes:
python
Copy code
python3 -c 'print(__import__("my_module").MyClass.__doc__)'
Functions (inside and outside a class):
python
Copy code
python3 -c 'print(__import__("my_module").my_function.__doc__)'
python
Copy code
python3 -c 'print(__import__("my_module").MyClass.my_function.__doc__)'
Python Unit Tests
unittest module
File extension .py
Files and folders start with test_
Organization: for models/base.py, unit tests in: tests/test_models/test_base.py
Execution command: python3 -m unittest discover tests
or: python3 -m unittest tests/test_models/test_base.py
Run Test in Interactive Mode:

bash
Copy code
echo "python3 -m unittest discover tests" | bash
Run Test in Non-interactive Mode:

bash
Copy code
python3 -m unittest discover tests
Usage
Start the console in interactive mode:

bash
Copy code
$ ./console.py
(hbnb)
Use help to see the available commands:

bash
Copy code
(hbnb) help

Documented commands (type help <topic>):
========================================
EOF  all  count  create  destroy  help  quit  show  update

(hbnb)
Quit the console:

bash
Copy code
(hbnb) quit
$
Commands
Create:

bash
Copy code
create <class>
bash
Copy code
(hbnb) create BaseModel
6cfb47c4-a434-4da7-ac03-2122624c3762
(hbnb)
Show:

bash
Copy code
show <class> <id>
bash
Copy code
(hbnb) show BaseModel 6cfb47c4-a434-4da7-ac03-2122624c3762
[BaseModel] (a) [BaseModel] (6cfb47c4-a434-4da7-ac03-2122624c3762) {'id': '6cfb47c4-a434-4da7-ac03-2122624c3762', 'created_at': datetime.datetime(2021, 11, 14, 3, 28, 45, 571360), 'updated_at': datetime.datetime(2021, 11, 14, 3, 28, 45, 571389)}
(hbnb)
Destroy:

bash
Copy code
(hbnb) create User
0c98d2b8-7ffa-42b7-8009-d9d54b69a472
(hbnb) destroy User 0c98d2b8-7ffa-42b7-8009-d9d54b69a472
(hbnb) show User 0c98d2b8-7ffa-42b7-8009-d9d54b69a472
** no instance found **
(hbnb)
All:

bash
Copy code
(hbnb) create BaseModel
e45ddda9-eb80-4858-99a9-226d4f08a629
(hbnb) all BaseModel
["[BaseModel] (4c8f7ebc-257f-4ed1-b26b-e7aace459897) [BaseModel] (4c8f7ebc-257f-4ed1-b26b-e7aace459897) {'id': '4c8f7ebc-257f-4ed1-b26b-e7aace459897', 'created_at': datetime.datetime(2021, 11, 13, 22, 19, 19, 447155), 'updated_at': datetime.datetime(2021, 11, 13, 22, 19, 19, 447257), 'name': 'My First Model', 'my_number': 89}"]
...
Count:

(hbnb) create City
4e01c33e-2564-42c2-b61c-17e512898bad
(hbnb) create City
e952b772-80a5-41e9-b728-6bc4dc5c21b4
(hbnb) count City
2
(hbnb)


Update:


(hbnb) create User
1afa163d-486e-467a-8d38-3040afeaa1a1
(hbnb) update User 1afa163d-486e-467a-8d38-3040afeaa1a1 email "aysuarex@gmail.com"
(hbnb) show User 1afa163d-486e-467a-8d38-3040afeaa1a1
[User] (s) [User] (1afa163d-486e-467a-8d38-3040afeaa1a1) {'id': '1afa163d-486e-467a-8d38-3040afeaa1a1', 'created_at': datetime.datetime(2021, 11, 14, 23, 42, 10, 502157), 'updated_at': datetime.datetime(2021, 11, 14, 23, 42, 10, 502186), 'email': 'aysuarex@gmail.com'}
(hbnb)




Authors
<details>
    <summary>Job Kimani</summary>
    <ul>
    <li><a href="https://github.com/jobkimani">Github</a></li>
    <li><a href="mailto:jobkimani29@gmail.com">E-mail</a></li>
    </ul>
</details>

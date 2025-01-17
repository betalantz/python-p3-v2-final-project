# Phase 3 Project: CLI and ORM

## Learning Goals

- Implement a Python application that includes a **Command Line Interface**.
- Implement a set of **Object-Relational Mapping** functions for two or more
  model classes.
- Define a Python object model that includes a one-to-many relationship between
  two classes.
- Exercise best practices in CLI design.
- Exercise best practices in OOP.

---

## Key Vocab

- **Command Line**: a text-based interface that is built into your computer's
  operating system. It allows you to access the files and applications on your
  computer manually or through scripts.
- **Terminal**: the application in Mac OS that allows you to access the command
  line.
- **Command Shell/Powershell**: the applications in Windows that allow you to
  access the command line.
- **Command-Line Interface (CLI)**: a text-based interface used to run programs,
  manage files and interact with objects in memory. As the name suggests, it is
  run from the command line.
- **Object-Relational Mapping (ORM)**: a programming technique that provides a
  mapping between an object-oriented data model and a relational database model.
- **Attribute**: variables that belong to an object.
- **Property**: attributes that are controlled by methods.
- **Decorator**: function that takes another function as an argument and returns
  a new function with added functionality.

---

## Introduction

Welcome to the end of Phase 3! You've learned about a lot in this unit:

- Python fundamentals.
- Data structures (and more recently, algorithms).
- Object-oriented programming.
- Object inheritance.
- Instance and class attributes and methods.
- Configuring applications.
- SQL fundamentals.
- Table relations in SQL.
- Object-relational mapping with Python.
- Building CLIs.

You're going to use these skills to create a CLI and ORM application. The Phase
3 project is open-ended when it comes to the actual content. You are free to
create whatever you'd like, as long as it incorporates the requirements listed
below.

## Requirements

You need to implement a Python CLI Application that meets the following
requirements.

### ORM Requirements

- The application must include a database created and modified with Python ORM
  methods using an ORM such as SQLAlchemy.

  - The data model must include **at least 2** model classes.
  - The data model must include **at least 1** one-to-many relationships.
  - Add appropriate constraints using the ORM to the columns on your data models.
  - Each model class should inherit from your ORM library.

### CLI Requirements

- The CLI must display menus with which a user may interact.
- The CLI should use loops as needed to keep the user in the application until
  they choose to exit.
- The CLI must include options: to create an object, delete an object,
  display all objects, view related objects, and find an object by attribute
  using ORM methods. These functions may be spread across different models.
- For **EACH** class in the data model, the CLI must at least read and display objects.
- The CLI should validate user input and object creations/deletions, providing
  informative errors to the user. In other words, no user input should cause the app
  to "error out" and crash to the prompt line, but should guide the user to inputting
  proper information.

# Project Environment, Configuration, Documentation

- The project code should follow OOP best practices.
- Pipfile contains all needed dependencies and no unneeded dependencies.
- Imports are used in files only where necessary.
- Project folders, files, and modules should be organized and follow appropriate
  naming conventions.
- The project should include a `README.md` that describes the application.

You do **not** need to implement tests for `pytest`, although you should test
your code thoroughly using your CLI. Try entering bad data when prompted for
input, and confirm your application prints a useful error message.

## How to begin?

- Start with the project template (provided in [this repo][template]). You are
  free to adapt the template structure, as long as you adhere to the project
  requirements.
- Think about the user interaction. How will you prompt the user? What
  information will the user enter? How will you provide feedback to the user?
- Think about your data model. How will you organize and store the information
  received from the user?
- If you get stuck trying to accomplish a specific task, check online to see if
  there's a Python library that will make it easier.
- Consider using [Click][click] or [Fire][fire] to take care of basic CLI tasks
  for you.

---

## Resources

- [Flatiron CLI Project Generator][template]
- [Click documentation][click]
- [The Python Fire Guide][fire]

[click]: https://click.palletsprojects.com/en/8.1.x/
[fire]: https://google.github.io/python-fire/guide/
[template]: https://github.com/learn-co-students/flatiron-cli-project-generator

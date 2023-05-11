# Lab_3_TMPS - Library App.
## by Agatiev Dumitru

## Task : 
    1. By creating a new project, or extending your last one (Lab work Nr2), implement at least 2 structural design patterns in your project

    2. Keep your files grouped (into packages/directories) by their responsibilities (an example project structure)

    3. Document your work in a separate markdown file according to the requirements presented below (the structure can be extended of course)

    4. Based on the previous point, implement at least 2 creational design patterns in your project.

## General Theory : 
Structural design patterns are a category of design patterns that focus on the composition of classes and objects to form larger structures and systems. They provide a way to organize objects and classes in a way that is both flexible and efficient, while allowing for the reuse and modification of existing code. Structural design patterns address common problems encountered in the composition of classes and objects, such as how to create new objects that inherit functionality from existing objects, how to create objects that share functionality without duplicating code, or how to define relationships between objects in a flexible and extensible way.

## Description :
As for what the app does, it is a simple command-line tool for managing a library. Users can add books to the library, list all the books in the library, rent a book, and return a book. When a book is rented, it is marked as unavailable until it is returned.

## Here is were these 4 patterns were used

   * Facade Pattern - This pattern provides a simple interface to a complex system, and hides the details of the system from the user. In this app, the LibraryFacade class serves as a facade for the Library class, providing simple methods to add and rent books.

   *  Adapter Pattern - This pattern allows incompatible interfaces to work together by providing a common interface. In this app, the LibraryAdapter and ISBNAdapter classes act as adapters between the Library and Book classes, allowing the LibraryFacade to work with books using ISBNs rather than directly working with the Book objects.

   * Decorator Pattern - This pattern adds behavior to an object dynamically, without affecting the behavior of other objects in the same class. In this app, the RentalDecorator class adds rental behavior to Book objects, without modifying the Book class itself.

   * Composite Pattern - This pattern allows you to compose objects into tree structures to represent part-whole hierarchies. In this app, the Library, Shelf, and Book classes are composed in a tree structure, where the Library contains multiple Shelf objects, and each Shelf object contains multiple Book objects.

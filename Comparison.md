# object-oriented-Language-Comparison

   [Go to README.md](README.md)
   
   [Go to code.txt](code.txt)
    
Compare Python and Java

    
* Errors and exception handling
    
    java:The error reporting functions allow you to customize what level and kind of error feedback is given, ranging from simple notices to customized functions returned during errors.
    
    python:It is possible to write programs that handle selected exceptions. Look at the following example, which asks the user for input until a valid integer has been entered, but allows the user to interrupt the program (using Control-C or whatever the operating system supports); note that a user-generated interruption is signalled by raising the KeyboardInterrupt exception.


* Lambda expressions, closures, or functions as types

  python: Python supports the creation of anonymous functions (i.e. functions that are not bound to a name) at runtime, using a construct called "lambda". This is not exactly the same as lambda in functional programming languages, but it is a very powerful concept that's well integrated into Python and is often used in conjunction with typical functional concepts like filter(), map() and reduce().

  java:a lambda function is an anonymous java function that can be stored in a variable and passed as an argument to other functions or methods. A closure is a lambda function that is aware of its surrounding context.

* Implementation of listeners and event handlers

  check code.txt please.

* Singleton
  * How is a singleton implemented?
  
    python:Possibly the simplest design pattern is the singleton, which is a way to provide one and only one object of a particular type. To accomplish this, you must take control of object creation out of the hands of the programmer. One convenient way to do this is to delegate to a single instance of a private nested inner class
    
    java:In the singleton pattern a class can distribute one instance of itself to other classes.
  
  * Can it be made thread-safe?
  
    java: yes, but your java version has to be thread-safe.
    
    python: yes
  
  * Can the singleton instance be lazily instantiated?
  
    python:yes
    
    java:yes
  
* Procedural programming
  * Does the language support procedural programming?
    
    python:yes
    
    java: yes
    
* Functional programming
  * Does the language support functional programming?
  
    python: yes, but it is not very good for functional programming.
    
    java:yes
    
* Multithreading
  * Threads or thread-like abilities
  
    python: only one thread can safely execute code in the interpreter at the same time.
    
    java: java is not a threaded language : its engine and its code don't manage threads to parallelize its own internal work. java doesn't offer threads to users : You can't use threads with the java language natively. 
  
  * How is multitasking accomplished?
    
    java: it hides the complex async work behind a promises-based interface.
    
    python: MultiTasking is a tiny Python library lets you convert your Python methods into asynchronous, non-blocking methods simply by using a decorator.
    
   [Go to README.md](README.md)
   
   [Go to code.txt](code.txt)

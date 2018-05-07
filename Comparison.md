

# object-oriented-Language-Comparison

   [Go to README.md](README.md)
   
   [Go to code.txt](code.txt)
    
Compare Python and Java

Group Member:

* Jiakang Yuchi

* Dongpeng Liu. pawprint: dltdc ID:14305410

---

* Language purpose/genesis
  * Why was the language created? 
  
    java: Because of the consumer electronics manufacturers market’s demand for CPU flexibility back in 1991, development need to be more platform-neutral process. The popular language at that time, C++, could not enable logic part to website pages. Java is intended to let application developers "write once, run anywhere", meaning that compiled Java code can run on all platforms that support Java without the need for recompilation, which enable Internet developers to explore without having to share their source code. 

    python: Python is a general-purpose programming language that emphasizes code readability, notably using significant whitespace. It enables clear programming on both small and large scales. 
    
  * What problems was the language trying to address? 
     
    java: Enable creation of applets for the World-Wide Web and make program portable and be able to operate in distributed environments. Besides, Java improved on simplicity compared to C/C++.
    
    python: The ancestor of Python, ABC language was lack of extensibility. At that time, the creator was working in the Amoeba distributed operating system group at CWI. Amoeba had its own system call interface which wasn’t easily accessible from the Bourne shell. Thus, Python was created, a scripting language with a syntax like ABC but with access to the Amoeba system. Moreover, instead of being an Amoeba-specific language, Python is generally extensible.
    
  * Is the language a reaction to a previous language or a replacement for another language?
   
    Java: Java derives much of its syntax from C and C++ but is with more high-level facilities.
    
    Python: 'A descendant of ABC that would appeal to Unix/C hackers.' , says the creator of Python, Guido van Rossum. Python is a successor to the ABC language and is capable of exception handling and interfacing with the Amoeba operating system. 
    
* Unique features of the language
  * Does the language have any particularly unique features? 
  
    Java: Java is Platform Independent by compiling in bytecode which can be interpreted on any system which have JVM; Java is Robust. It has the strong memory allocation and automatic garbage collection mechanism; Java is multithreaded.
    
    Python: Python is easy to code and read. Its formatting is visually uncluttered, and it often uses English keywords where other languages use punctuation ; Python was designed to be highly extensible, which enables adding programmable interfaces to existing applications; Coding methodology of Python: "there should be one—and preferably only one—obvious way to do it"; Python comes with a large standard library that covers areas such as string processing (regular expressions, Unicode, calculating differences between files), Internet protocols (HTTP, FTP, SMTP, XML-RPC, POP, IMAP, CGI programming), software engineering (unit testing, logging, profiling, parsing Python code), and operating system interfaces (system calls, filesystems, TCP/IP sockets).

* Name spaces
  * How are name spaces implemented?
      
    Java: In Java, the idea of a namespace is embodied in Java packages. 
    
    Python: Python implements namespaces as dictionaries. There is a name-to-object mapping, with the names as keys and the objects as values. Multiple namespaces can use the same name and map it to a different object.
    
  * How are name spaces used?
  
    Java: All code belongs to a package, although that package need not be explicitly named. Code from other packages is accessed by prefixing the package name before the appropriate identifier.
    
    Python: Local Namespace is created when a function is called, and it only lasts until the function returns; Global Namespace is created when the module is included in the project, and it lasts until the script ends; Built-in Namespace includes built-in functions and built-in exception names.

* Types
  * What types does the language support?
  
    Java: boolean, char, byte, integral including byte, int, long, short and floating-point types including float and double.
    
    Python: Python is dynamically-typed. This means that the type for a value is decided at runtime, not in advance. Python's Built-in Data types include numeric types (int, long , float, complex), boolean, sequences (str, bytes, byte, list, tuple), sets, mappings and some others such as type and callables.
    
  * Are both reference and value types supported?
  
    Java: Yes.
    
    Python: No. Python is neither "call-by-value" or "call-by-reference". It is a "call-by-object" model, which means In Python a variable is not an alias for a location in memory. Rather, it is simply a binding to a Python object.
    
  * Can new value types be created?
  
    Java: No.
    
    Python: Yes, Python allows programmers to define their own types using classes.
  
* Classes

  * Defining

    Java:
    ```java
    class MyClass extends MySuperClass implements YourInterface {
      ...
    }
    ```

    Python 3:

    ```python
    class DerivedClassName(superClass1, superClass2, superClass3):
        ...
    ```

  * Creating new instances

    Java: There are three steps when creating an object from a class −

    Declaration − A variable declaration with a variable name with an object type.

    Instantiation − The 'new' keyword is used to create the object.

    Initialization − The 'new' keyword is followed by a call to a constructor. This call initializes the new object.

    ```java
     public class Puppy {
       public Puppy(String name) {
          // This constructor has one parameter, name.
          System.out.println("Passed Name is :" + name );
       }

       public static void main(String []args) {
          // Following statement would create an object
          Puppy myPuppy = new Puppy( "tommy" );
       }
     }
    ```

    Python: Class instantiation uses function notation. We can treat the class object as a parameterless function that returns a new instance of the class.

    ```python
    x = MyClass()
    ```

  * Constructing/initializing

    Java: Instantiation − The 'new' keyword is used to create the object. Constructing - Java compiler builds a default constructor for that class. Each time a new object is created, at least one constructor will be invoked. The main rule of constructors is that they should have the same name as the class. A class can have more than one constructor.

    ```java
    public class Puppy {
      //constructors
      public Puppy()
      public Puppy(String name)
    }
    ```

    python: When a class have a `def __init__()` method, class instantiation automatically invokes this initializing method for the newly-created class instance. So a new, initialized instance can be obtained by `x = MyClass()`.

  * Destructing/de-initializing

    Java: Because Java is a garbage collected language we cannot predict when (or even if) an object will be destroyed. Hence there is no direct equivalent of a destructor. We can use method `public void finalize()` instead.

    python: In Python, destructors are needed much less, because Python has a garbage collector that handles memory management. Python has the destructor concept - the `__del__()` method.

* Instance reference name in data type (class)

  * this? self?

    Java uses this and python uses self for instance reference. Both `Bound Method` and `Unbound Method` are supported in python.

* Properties

  * Getters and setters…write your own or built in?

    Java: write your own getters and setters methods.

    python: We can write own code for setter and getter, or use the properties.

    ```python
    @property
    def x(self):
        return self.__x

    @x.setter
    def x(self, x):
      ...
    ```

  * Backing variables?

    Both Java and Python are supported variables as properties.

  * Computed properties?

    A computed attribute (or "managed attribute") looks like it directly accesses storage, but works like a function. That is, you code a computed attribute without parentheses or arguments, but accessing the attribute causes a function to be executed.

    Java: Yes. When we use a custom getter and/or setter method with a variable, it is a computed property, as opposed to a stored property.

    python: supported.
    '''python
    save_me = wgt.color
    top_edge_color = (255,) + wgt.color[1:]
    ```

* Interfaces / protocols

  * What does the language support?

    Java: Interfaces. It has static constants and abstract methods. The interface in java is a mechanism to achieve abstraction. There can be only abstract methods in the java interface. It is used to achieve abstraction and multiple inheritance in Java.

    Python: Interfaces are not necessary in Python. This is because Python has proper multiple inheritanc

  * What abilities does it have?

    Java: A very common use of interfaces is for listeners. A listener is an object from a class that implements the required methods for that interface. Interfaces replace multiple inheritance.

    python: More commonly Python coders prefer to use the richer concept known as an "Abstract Base Class" (ABC), which combines an interface with the possibility of having some implementation aspects there too.

  * How is it used?

    Java: Widly used.

    Python: Not common. There are third-party implementations of interfaces for Python (most popular is Zope's, also used in Twisted)

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

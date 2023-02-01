## Python OOP Assignment
Q1. What is the purpose of Python's OOP?

Ans - In Python, object-oriented Programming (OOPs) is a programming paradigm that uses objects and classes in programming. It aims to implement real-world entities like inheritance, polymorphisms, encapsulation, etc. in the programming. The main concept of OOPs is to bind the data and the functions that work on that together as a single unit so that no other part of the code can access this data.

Q2. Where does an inheritance search look for an attribute?

Ans - An inheritance search looks for an attribute first in the instance object, then in the class the instance was created from, then in all higher superclasses, progressing from left to right (by default). The search stops at the first place the attribute is found.

Q3. How do you distinguish between a class object and an instance object?

Ans - 	            Object	                                                            Class
 1)	Object is an instance of a class.	                               Class is a blueprint or template from which objects are created.
 2)	Object is a real world entity such as pen, laptop, etc.	           Class is a group of similar objects.
 3)	Object is a physical entity.	                                   Class is a logical entity.
 4)	Object is created through new keyword mainly e.g. 
    Student s1=new Student();	                                       Class is declared using class keyword e.g.class Student{}
 5)	Object is created many times as per requirement.	               Class is declared once.
 6)	Object allocates memory when it is created.	                       Class doesn't allocated memory when  it is created.
 7)	There are many ways to create object in java                       There is  only one way to define class in java using class keyword.
    such as new keyword, newInstance() method, clone() method, 
    factory method and deserialization.

Q4. What makes the first argument in a class’s method function special?

Ans - Often, the first argument of a method is called self.This is nothing more than a convention: the name self has absolutely no special meaning to Python.  
The self is used to represent the instance of the class. With this keyword, you can access the attributes and methods of the class in python. It binds the attributes with the given arguments. The reason why we use self is that Python does not use the ‘@’ syntax to refer to instance attribute.

Q5. What is the purpose of the init method?

Ans - The Default __init__ Constructor in C++ and Java. Constructors are used to initializing the object’s state. The task of constructors is to initialize(assign values) to the data members of the class when an object of the class is created. Like methods, a constructor also contains a collection of statements(i.e. instructions) that are executed at the time of Object creation. It is run as soon as an object of a class is instantiated. The method is useful to do any initialization you want to do with your object.

# A Sample class with init method
class Person:
 
    # init method or constructor
    def __init__(self, name):
        self.name = name
 
    # Sample Method
    def say_hi(self):
        print('Hello, my name is', self.name)
 
 
p = Person('Nikhil')
p.say_hi()

In the above example, a person name Nikhil is created. While creating a person, “Nikhil” is passed as an argument, this argument will be passed to the __init__ method to initialize the object. The keyword self represents the instance of a class and binds the attributes with the given arguments. Similarly, many objects of the Person class can be created by passing different names as arguments.

Q6. What is the process for creating a class instance?

Ans - To create instances of a class, you call the class using class name and pass in whatever arguments its __init__ method accepts.

"This would create first object of Employee class"
emp1 = Employee("Zara", 2000)
"This would create second object of Employee class"
emp2 = Employee("Manni", 5000)

You access the object's attributes using the dot operator with object. Class variable would be accessed using class name as follows −

emp1.displayEmployee()
emp2.displayEmployee()
print "Total Employee %d" % Employee.empCount

Q7. What is the process for creating a class?

Ans - In Python, a class can be created by using the keyword class, followed by the class name. The syntax to create a class is given below.

class ClassName:    

Q8. How would you define the superclasses of a class?

Ans -  A class that is derived from another class is called a subclass (also a derived class, extended class, or child class). The class from which the subclass is derived is called a superclass (also a base class or a parent class).

Q9. What is the relationship between classes and modules?

Ans - Modules in Python are files with a .py extension using which we can reuse elements inside that file.
If we want to reuse the same piece of function code or the same class, rewriting it would make our code redundant and repetitive. Instead, we can import that entire file as a module into another program. 

Q10. How do you make instances and classes?

Q11. Where and how should be class attributes created?

Ans - Class attributes are the variables defined directly in the class that are shared by all objects of the class. Instance attributes are attributes or properties attached to an instance of a class. Instance attributes are defined in the constructor. Defined directly inside a class.

Q12. Where and how are instance attributes created?

Ans - Instance attributes are defined in the constructor. Defined directly inside a class. Defined inside a constructor using the self parameter.

 # init method or constructor
    def __init__(self, name):
        self.name = name


Q13. What does the term "self" in a Python class mean?

Ans - The self parameter is a reference to the current instance of the class, and is used to access variables that belongs to the class.

Q14. How does a Python class handle operator overloading?

Ans - 
In Python, overloading is achieved by overriding the method which is specifically for that operator, in the user-defined class. For example, __add__(self, x) is a method reserved for overloading + operator, and __eq__(self, x) is for overloading == .

The operator overloading in Python means provide extended meaning beyond their predefined operational meaning. Such as, we use the "+" operator for adding two integers as well as joining two strings or merging two lists. We can achieve this as the "+" operator is overloaded by the "int" class and "str" class.

Q15. When do you consider allowing operator overloading of your classes?

Ans - Operator overloading is mostly useful when you're making a new class that falls into an existing "Abstract Base Class" (ABC) 

Q16. What is the most popular form of operator overloading?

Ans - A very popular and convenient example is the Addition (+) operator. Just think how the '+' operator operates on two numbers and the same operator operates on two strings. It performs “Addition” on numbers whereas it performs “Concatenation” on strings.

Q17. What are the two most important concepts to grasp in order to comprehend Python OOP code?

Ans - Both inheritance and polymorphism are fundamental concepts of object oriented programming. These concepts help us to create code that can be extended and easily maintainable.

Q18. Describe three applications for exception processing.

Ans - Raised when the specified key is not found in the dictionary. Raised when an identifier is not found in the local or global namespace. Raised when trying to access a local variable in a function or method but no value has been assigned to it. Base class for all exceptions that occur outside the Python environment.

Q19. What happens if you don't do something extra to treat an exception?

Ans - When an exception occurred, if you don't handle it, the program terminates abruptly and the code past the line that caused the exception will not get executed.

Q20. What are your options for recovering from an exception in your script?

Ans - You can also provide a generic except clause, which handles any exception. After the except clause(s), you can include an else-clause. The code in the else-block executes if the code in the try: block does not raise an exception. The else-block is a good place for code that does not need the try: block's protection.

Q21. Describe two methods for triggering exceptions in your script.

Ans - To avoid such a scenario, there are two methods to handle Python exceptions: 
Try – This method catches the exceptions raised by the program. 
Raise – Triggers an exception manually using custom exceptions.

Q22. Identify two methods for specifying actions to be executed at termination time, regardless of  
whether or not an exception exists.

Ans - 

Q23. What is the purpose of the try statement?

Ans - 
The try and except block in Python is used to catch and handle exceptions. Python executes code following the try statement as a “normal” part of the program. The code that follows the except statement is the program's response to any exceptions in the preceding try clause.

Q24. What are the two most popular try statement variations?

Ans -  There are two other optional segments to a try block: else and finally . Both of these optional blocks will come after the try and the except 

Q25. What is the purpose of the raise statement?

Ans - The raise keyword is used to raise an exception. You can define what kind of error to raise, and the text to print to the user.

Q26. What does the assert statement do, and what other statement is it like?

Ans - 
Python's assert statement allows you to write sanity checks in your code. These checks are known as assertions, and you can use them to test if certain assumptions remain true while you're developing your code. If any of your assertions turn false, then you have a bug in your code.

Q27. What is the purpose of the with/as argument, and what other statement is it like?

Ans - The with statement is a replacement for commonly used try/finally error-handling statements. A common example of using the with statement is opening a file. To open and write to a file in Python.

Q28. What are *args, **kwargs?

Ans - 

Variable-length/ Arbitrary arguments in Python (*args)

When you don’t know in advance about the number of arguments to be passed, the arguments are variable-length. Include an asterisk i.e. * before the parameter name while defining the function. Let us see an example:

def demo(*car):
   print("Car 1 = ",car[0])
   print("Car 2 = ",car[1])
   print("Car 3 = ", car[2])
   print("Car 4 = ", car[3])

# call
demo("Tesla", "Audi", "BMW", "Toyota")

Output
('Car 1 = ', 'Tesla')
('Car 2 = ', 'Audi')
('Car 3 = ', 'BMW')
('Car 4 = ', 'Toyota')

Arbitrary Keyword Arguments in Python (**kwargs)

When you don’t know in advance about the number of keyword arguments to be passed, the arguments are arbitrary keyword arguments.

Example
Let us see an example −

def demo(**c):
   print("Car Name: "+c["name"])
   print("Car Model: "+c["model"])

# call
demo(name = "Tesla", model = "2022")
Output
Car Name: Tesla
Car Model: 2022

Q29. How can I pass optional or keyword parameters from one function to another?

Ans - 
Pass optional or keyword parameters from one function to another
To pass, collect the arguments using the * and ** in the function’s parameter list. Through this, you will get the positional arguments as a tuple and the keyword arguments as a dictionary. Pass these arguments when calling another function by using * and ** −

def f(a, *args, **kwargs):
   ...
   kwargs['width'] = '14.3c'
   ...
   g(a, *args, **kwargs)


Q30. What are Lambda Functions?

Ans - 
A lambda function is an anonymous function (i.e., defined without a name) that can take any number of arguments but, unlike normal functions, evaluates and returns only one expression. A lambda function in Python has the following syntax: lambda parameters: expression.

Q31. Explain Inheritance in Python with an example?

Ans - Inheritance is the capability of one class to derive or inherit the properties from another class. The class that derives properties is called the derived class or child class and the class from which the properties are being derived is called the base class or parent class.

# Python code to demonstrate how parent constructors
# are called.
 
# parent class
class Person(object):
 
    # __init__ is known as the constructor
    def __init__(self, name, idnumber):
        self.name = name
        self.idnumber = idnumber
 
    def display(self):
        print(self.name)
        print(self.idnumber)
         
    def details(self):
        print("My name is {}".format(self.name))
        print("IdNumber: {}".format(self.idnumber))
     
# child class
class Employee(Person):
    def __init__(self, name, idnumber, salary, post):
        self.salary = salary
        self.post = post
 
        # invoking the __init__ of the parent class
        Person.__init__(self, name, idnumber)
         
    def details(self):
        print("My name is {}".format(self.name))
        print("IdNumber: {}".format(self.idnumber))
        print("Post: {}".format(self.post))
 
 
# creation of an object variable or an instance
a = Employee('Rahul', 886012, 200000, "Intern")
 
# calling a function of the class Person using
# its instance
a.display()
a.details()

Output - 
Rahul
886012
My name is Rahul
IdNumber: 886012
Post: Intern

we have created two classes i.e. Person (parent class) and Employee (Child Class). The Employee class inherits from the Person class. We can use the methods of the person class through employee class as seen in the display function in the above code. A child class can also modify the behavior of the parent class as seen through the details() method.

Q32. Suppose class C inherits from classes A and B as class C(A,B).Classes A and B both have their own versions of method func(). If we call func() from an object of 
class C, which version gets invoked?

Ans - Both

Q33. Which methods/functions do we use to determine the type of instance and inheritance?

Ans - 
The isinstance() method checks whether an object is an instance of a class whereas issubclass() method asks whether one class is a subclass of another class (or other classes)

isinstance(object, classinfo)
Return true if the object argument is an instance of the classinfo argument, or of a (direct, indirect or virtual) subclass thereof.

issubclass(class, classinfo)
Return true if class is a subclass (direct, indirect or virtual) of classinfo. A class is considered a subclass of itself.

example -  
class MyClass(object):
  pass
class MySubClass(MyClass):
  pass
print(isinstance(MySubClass, object))
print(issubclass(MySubClass, MyClass))
print(isinstance(MySubClass, MyClass))

Output-
True
True
False

Q34.Explain the use of the 'nonlocal' keyword in Python.

Ans - The nonlocal keyword won’t work on local or global variables and therefore must be used to reference variables in another scope except the global and local one. The nonlocal keyword is used in nested functions to reference a variable in the parent function. 

Q35. What is the global keyword?

Ans - A global keyword is a keyword that allows a user to modify a variable outside the current scope.

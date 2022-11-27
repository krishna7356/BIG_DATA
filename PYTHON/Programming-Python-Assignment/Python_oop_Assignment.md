## Python OOP Assignment
Q1. What is the purpose of Python's OOP?
ans:Python is also an object-oriented language since its beginning. It allows us to develop applications using an Object-Oriented approach. In Python, we can easily create and use classes and objects.An object-oriented paradigm is to design the program using classes and objects. The object is related to real-word entities such as book, house, pencil, etc. The oops concept focuses on writing the reusable code. It is a widespread technique to solve the problem by creating objects.Major principles of object-oriented programming system are Class,Object,Method,Inheritance,Polymorphism,Data abstraction,Encapsulation.

Q2. Where does an inheritance search look for an attribute?
ans:The inheritance search is simply a search of the tree from bottom to top looking for the lowest occurrence of an attribute name. Code implies the shape of such trees.

Q3. How do you distinguish between a class object and an instance object?
ans:Class object is An Object is an instance of a Class. A class is like a blueprint while an instance is a copy of the class with actual values.
An object consists of : 

*State: It is represented by the attributes of an object. It also reflects the properties of an object.
*Behaviour: It is represented by the methods of an object. It also reflects the response of an object to other      objects.
*Identity: It gives a unique name to an object and enables one object to interact with other objects.

Instance object :
Instance variables are for data, unique to each instance and class variables are for attributes and methods shared by all instances of the class. Instance variables are variables whose value is assigned inside a constructor or method with self whereas class variables are variables whose value is assigned in the class.

Q4. What makes the first argument in a class’s method function special?
ans: The self parameter is a reference to the current instance of the class, and is used to access variables that belongs to the class.It's the frist argument in the class method.

Q5. What is the purpose of the init method?
ans: The Default __init__ Constructor in C++ and Java. Constructors are used to initializing the object’s state. The task of constructors is to initialize(assign values) to the data members of the class when an object of the class is created. Like methods, a constructor also contains a collection of statements(i.e. instructions) that are executed at the time of Object creation. It is run as soon as an object of a class is instantiated. The method is useful to do any initialization you want to do with your object.

Q6. What is the process for creating a class instance?
ans: all you have to do to create a new instance of a class in Python is choose a name for the object and set it equal to the class name (that you created) followed by ().When referencing a class in Python, it should always be the class name with parenthesis ().
eg:-class Person:  
    # init method or constructor   
    def __init__(self, name):  
        self.name = name  
      
    # Sample Method   
    def say_hi(self):  
        print('Hello, my name is', self.name)  
      
p = Person('Nikhil')  
p.say_hi()

Q7. What is the process for creating a class?
ans: 
* Classes are created by keyword class.
*Attributes are the variables that belong to a class.
*Attributes are always public and can be accessed using the dot (.) operator.
eg:-
class Dog:
    pass
 the class keyword indicates that you are creating a class followed by the name of the class (Dog in this case).

Q8. How would you define the superclasses of a class?
ans: Syntax: super()
Return : Return a proxy object which represents the parent’s class.
eg:-
class Person:
	# Constructor
	def __init__(self, name, id):
		self.name = name
		self.id = id
	# To check if this person is an employee
	def Display(self):
		print(self.name, self.id)
class Emp(Person):
	def __init__(self, name, id):
		self.name_ = name
		super().__init__(name, id)
	def Print(self):
		print("Emp class called")
Emp_details = Emp("Mayank", 103)
#calling parent class function
print(Emp_details.name_, Emp_details.name)

Q9. What is the relationship between classes and modules?
ans:The difference between a class and a module in python is that a class is used to define a blueprint for a given object, whereas a module is used to reuse a given piece of code inside another program.
A class can have its own instance, but a module cannot be instantiated. We use the ‘class’ keyword to define a class, whereas to use modules, we use the ‘import’ keyword. We can inherit a particular class and modify it using inheritance. But while using modules, it is simply a code containing variables, functions, and classes.
Modules are files present inside a package, whereas a class is used to encapsulate data and functions together inside the same unit

Q10. How do you make instances and classes?
ans:In Python Programming Language, Class and Instance are two of object orientation's most crucial ideas. Instances are unique objects made in accordance with the class, whereas classes are templates. The procedure is the same for all objects, although the data may vary.

Q11. Where and how should be class attributes created?
ans: A class attribute is shared by all instances of the class.Use class_name.class_attribute or object_name.class_attribute to access the value of the class_attribute.Use class attributes for storing class contants, track data across all instances, and setting default values for all instances of the class.
eg:-
class Test:
    x = 10
    def __init__(self):
        self.x = 20
print(Test.x)  # 10

Q12. Where and how are instance attributes created?
ans: Instances are unique objects made in accordance with the class,instance attributes are created inside the class.
Q13. What does the term "self" in a Python class mean?
ans:self represents the instance of the class. By using the “self” keyword we can access the attributes and methods of the class in python. It binds the attributes with the given arguments.
Q14. How does a Python class handle operator overloading?
ans: Python operators work for built-in classes. But the same operator behaves differently with different types. For example, the + operator will perform arithmetic addition on two numbers, merge two lists, or concatenate two strings

Q15. When do you consider allowing operator overloading of your classes?
ans: Operator overloading is helpful in cases where the operators used for certain types provide semantics related to the domain context and syntactic support as found in the programming language. It is used for syntactical convenience, readability and maintainability.

Q16. What is the most popular form of operator overloading?
ans: The most frequent instance is the adding up operator ‘+’, where it can be used for the usual addition and also for combining two different strings.

Q17. What are the two most important concepts to grasp in order to comprehend Python OOP code?
ans:  Inheritance and polymorphism are fundamental concepts of object oriented programming.
Q18. Describe three applications for exception processing.
ans:  
*Library :A library is a set of functions / classes focusing on some problem domain.Libraries do not control the flow of program. Functions of libraries are called by the main program with some input and they return some output or provide some behavior.
*API : APIs can be thought of as a library of functions exposed over a network e.g., continuing earlier example, if there is a decision to expose the Data Access APIs as REST APIs.framework must handle exception in all the places where it is invoking methods on its plug-in.Framework itself cannot be the reason for a crash so it must also make sure that it internally doesn't allow any exception to go unhandled and reach the runtime because that may result in a crash.
*UI Application :Almost all UI applications are written using some framework with the framework calling the application when there is some event. This makes the event handlers an entry point in to the application so exceptions should be caught on event handlers.

Q19. What happens if you don't do something extra to treat an exception?
ans:If you do nothing, the exception causes your application to crash. Or you can choose to handle the exception. That is, you acknowledge that the problem happened, prevent the application from crashing, and take the steps necessaries in order to either recover from the error or fail gracefully.

Q20. What are your options for recovering from an exception in your script?
ans:try/except: catch the error and recover from exceptions hoist by programmers or Python itself.

Q21. Describe two methods for triggering exceptions in your script.
ans: Common triggering exceptions ZeroDivisionError,NameError,IndentationError

Q22. Identify two methods for specifying actions to be executed at termination time, regardless of  whether or not an exception exists.
ans: The process termination mechanism in Python is implemented by throwing a SystemExit exception.Terminate a Program Using the quit() Function The quit()function is an inbuilt function

Q23. What is the purpose of the try statement?
ans:The try block is used to check some code for errors i.e the code inside the try block will execute when there is no error in the program. Whereas the code inside the except block will execute whenever the program encounters some error in the preceding try block.

Q24. What are the two most popular try statement variations?
ans : 
*  try/except:
try:
    statement(s)
except [expression [, target]]:
    statement(s)
[else:
    statement(s)]
Try Except in Python Try and Except statement is used to handle these errors within our code in Python. The try block is used to check some code for errors i.e the code inside the try block will execute when there is no error in the program.
*try/finally
try:
    statement(s)
finally:
    statement(s)
finally block is always executed after leaving the try statement. In case if some exception was not handled by except block, it is re-raised after execution of finally block.

Q25. What is the purpose of the raise statement?
ans:Introduction to the Python raise statement To raise an exception, you use the raise statement: raise ExceptionType ().

Q26. What does the assert statement do, and what other statement is it like?
ans: The assert Statements in Python The assert statement checks if a condition evaluates True. If it does, the program keeps running. If it does not, the program returns an AssertionError and the program stops executing.
assert is also act like if statement ,if it's True program run.

Q27. What is the purpose of the with/as argument, and what other statement is it like?
ans: with statement is used in exception handling to make the code cleaner and much more readable.as means it used for aliasing the name.
eg: # using with statement
with open('file_path', 'w') as file:
    file.write('hello world !')

Q28. What are *args, **kwargs?
ans: *args in function definitions in python is used to pass a variable number of arguments to a function. It is used to pass a non-key worded, variable-length argument list. 
**kwargs in function definitions in python is used to pass a keyworded, variable-length argument list. We use the name kwargs with the double star. The reason is that the double star allows us to pass through keyword arguments (and any number of them).

Q29. How can I pass optional or keyword parameters from one function to another?
ans:To pass, collect the arguments using the * and ** in the function’s parameter list. Through this, you will get the positional arguments as a tuple and the keyword arguments as a dictionary. Pass these arguments when calling another function by using * and ** .
eg:
def f(a, *args, **kwargs):
   ...
   kwargs['width'] = '14.3c'
   ...
   g(a, *args, **kwargs)

Q30. What are Lambda Functions?
ans:Lambda Functions are anonymous function means that the function is without a name.The lambda keyword is used to define an anonymous function in Python.This function can have any number of arguments but only one expression, which is evaluated and returned.One is free to use lambda functions wherever function objects are required.You need to keep in your knowledge that lambda functions are syntactically restricted to a single expression.It has various uses in particular fields of programming, besides other types of expressions in functions

Q31. Explain Inheritance in Python with an example?
ans:inheritance is a mechanism that allows you to create a hierarchy of classes that share a set of properties and methods by deriving a class from another class. Inheritance is the capability of one class to derive or inherit the properties from another class.
eg:- 
class Person(object):
#Constructor
	def __init__(self, name):
		self.name = name

	# To get name
	def getName(self):
		return self.name

	# To check if this person is an employee
	def isEmployee(self):
		return False
#Inherited or Subclass (Note Person in bracket)
class Employee(Person):

	# Here we return true
	def isEmployee(self):
		return True
emp = Person("Rahul") # An Object of Person
print(emp.getName(), emp.isEmployee())

emp = Employee("manohar") # An Object of Employee
print(emp.getName(), emp.isEmployee())

Q32. Suppose class C inherits from classes A and B as class C(A,B).Classes A and B both have their own versions of method func(). If we call func() from an object of 
class C, which version gets invoked?
ans: class A version func() is invoke.

Q33. Which methods/functions do we use to determine the type of instance and inheritance?
ans: The isinstance() method checks whether an object is an instance of a class whereas issubclass() method asks whether one class is a subclass of another class (or other classes).

Q34.Explain the use of the 'nonlocal' keyword in Python.
ans:Python nonlocal keyword is used to reference a variable in the nearest scope. 
eg:
def foo():
	name = "good" # Our local variable

	def bar():
		nonlocal name		 # Reference name in the upper scope
		name = 'Good morning' # Overwrite this variable
		print(name)
		
	# Calling inner function
	bar()
	
	# Printing local variable
	print(name)

foo()
output  : Good morning
		  Good morning

Q35. What is the global keyword?
ans: A global keyword is a keyword that allows a user to modify a variable outside the current scope. It is used to create global variables in Python from a non-global scope, i.e. inside a function. Global keyword is used inside a function only when we want to do assignments or when we want to change a variable. Global is not needed for printing and accessing.
eg:
x = 15
def change():
	# using a global keyword
	global x
	# increment value of a by 5
	x = x + 5
	print("Value of x inside a function :", x)
change()
print("Value of x outside a function :", x)
 output:-
Value of x inside a function : 20
Value of x outside a function : 20
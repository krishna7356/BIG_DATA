## Assignment Part-1
Q1. Why do we call Python as a general purpose and high-level programming language?

ans: Python is a high-level language which means that it's simpler and more intuitive for human use.low-level language like c\c++ required more understanding about how computer works but in high-level language,many of details are abstracted and it make life easier.
Python is a general-purpose language which means it can be used for a wide variety of development tasks. Unlike a domain-specific language that can only be used for specific types of applications ( JavaScript and HTML/CSS for web development....)
Q2. Why is Python called a dynamically typed language?

ans: We don't have to declare the type of variable while assigning a value to a variable in Python. Other languages like C, C++, Java, etc.., there is a strict declaration of variables before assigning values to them.Python don't have any problem even if we don't declare the type of variable. It states the kind of variable in the runtime of the program.

Q3. List some pros and cons of Python programming language?
anss:
    pros
 * Python is very easy to learn and read.
 * Python enhance the productivity
 * Python has vast collection  of libraries
 * Pyhton is free,open source,has a very large community
 * Python is a interpreted language

    cons
* Python has speed limitation
* Python can have runtime error
* Python comes out a lot of memory space
* Python is not easy to test


Q4. In what all domains can we use Python?
ans:
* Machine learning / Artificial intelligence
* Desktop GUI
* Data anaiytical and Data visualization
* Web development
* Game development
* Embedded systems
Q5. What are variable and how can we declare them?

ans:Python has no command for declaring a variable. A variable is created when some value is assigned to it. The value assigned to a variable determines the data type of that variable.

Q6. How can we take an input from the user in Python?

ans: In Python we can use the input() method to take user input.After taking input ,input() method return the entered value as string.

Q7. What is the default datatype of the value that has been taken as an input using input() function?

ans: String 

Q8. What is type casting?

ans: Type conversion is the process of converting an object's data type from its original data type to our required data type

Q9. Can we take more than one input from the user using single input() function? If yes, how? If no, why?
ans: yes,we can input mulitiple input using a single input() function .we can use split() method to split out input and it store in list format
Q10. What are keywords?
ans: key words in pyhton are assert,in,del,and,else,raise,from,if,continue,not,pass,finally,while,yield,is,as,break,return,elif,except,def,global,import,for,exec,or,print,lambda,with,class,try.

Q11. Can we use keywords as a variable? Support your answer with reason.
ans: No,it can not use as a variable name or any other identifier name.Keywords are reserved words in Python and used to perform an internal operations.

Q12. What is indentation? What's the use of indentaion in Python?
ans: Python indentation refers to adding white space before a statement to a particular block of code. In another word, all the statements with the same space to the right, belong to the same code block.

Q13. How can we throw some output in Python?
ans: We can use print() function to display the output.

Q14. What are operators in Python?
ans:
* Arithmetic Operators 
   + -->  Add 
   - -->  subtraction
   * -->  Multiplication
   / -->  Division
   % -->  Modulus
   ** ->  Exponent
   // ->  Floor Division

* Assignment Operators
   =    Equal	
   +=   Add AND	
   -=   Subtract AND	
   *=   Multiply AND	
   %=   Modulus AND
   **=  Exponent AND
   //=  Floor Division AND

* Comparison Operators
   ==	Double Equal
   != 	Not Equal To
   >	Greater Than	 
   <	Less Than	
   <=	Less Than Equal To
   >=	Greater Than Equal To

* Logical Operators
   or	Logical OR	
   and	Logical AND	
   not	Logical NOT

Q15. What is difference between / and // operators?
ans: '/' Float division --> Divides left hand side by right hand side
eg: 5/2 --> 2.5
'//' Integer division --> divides left hand side by right hand side and remove the decimal point
eg: 5//2 --> 2 

Q16. Write a code that gives following as an output.
```
iNeuroniNeuroniNeuroniNeuron
```
ans: print("iNeuron"*4)
Q17. Write a code to take a number as an input from the user and check if the number is odd or even.
ans:
number = int(input("Enter the number: ))
if (number % 2==0):         # checking the number is even 
    print(f"{number} is even number)
else:
    print(f"{number} is odd number")

Q18. What are boolean operator?

Q19. What will the output of the following?
```
1 or 0
ans : 1

0 and 0
ans: 0

True and False and True
ans: False

1 or 0 or 0
ans :1
```

Q20. What are conditional statements in Python?
ans: Python program, the conditional statement is how you perform this sort of decision-making. It allows for conditional execution of a statement or group of statements based on the value of an expression.

Q21. What is use of 'if', 'elif' and 'else' keywords?
ans: The if / elif / else structure is a common way to control the flow of a program, allowing you to execute specific blocks of code depending on the value of some data. if statement If the condition following the keyword if evaluates as true, the block of code will execute.

Q22. Write a code to take the age of person as an input and if age >= 18 display "I can vote". If age is < 18 display "I can't vote".
ans:
age = int(input("Enter the age : "))
if(age >= 18): # checking age greater than or equal to 18
    print("I can vote ")
else:           # age is less than 18
    print("I can't vote")


Q23. Write a code that displays the sum of all the even numbers from the given list.
```
numbers = [12, 75, 150, 180, 145, 525, 50]
```
ans:
sum=0  # store the sum of elements 
for number in numbers:  # itreate threw all elements in list
    if(number % 2==0):  # check the number is even
        sum +=number    # suming the even numbers
print("Sum of all the Even number : ",sum )


Q24. Write a code to take 3 numbers as an input from the user and display the greatest no as output.
ans:
number_1=int(input("Enter number : "))
number_2=int(input("Enter number : "))
number_3=int(input("Enter number : "))
if(number_1 > number_2) and (number_1>number_3):
    print(f"{number_1} is the greatest number")
elif(number_2>number_3):
    print(f"{number_2} is the greatest number")
elif(number_3>number_2):
    print(f"{number_3} is the greatest number")

Q25. Write a program to display only those numbers from a list that satisfy the following conditions

- The number must be divisible by five

- If the number is greater than 150, then skip it and move to the next number

- If the number is greater than 500, then stop the loop
```
numbers = [12, 75, 150, 180, 145, 525, 50]
```
ans:
for number in numbers:
    if(number%5==0):
        if(number>500):
            break
        elif(number >150):
            continue
        else:
            print(number)
Q26. What is a string? How can we declare string in Python?
ans:Strings in Python are arrays of bytes representing unicode characters.Strings in python are surrounded by either single quotation marks, or double quotation marks.'hello' is the same as "hello".

Q27. How can we access the string using its index?
ans: 
a = "Hello, World!"
print(a[1])
Q28. Write a code to get the desired output of the following
```
string = "Big Data iNeuron"
desired_output = "iNeuron"
```
ans:
string = "Big Data iNeuron"
desired_output = string[9:]
print(desired_output)

Q29. Write a code to get the desired output of the following
```
string = "Big Data iNeuron"
desired_output = "norueNi"
```
ans:
string = "Big Data iNeuron"
desired_output = string[-1:-8:-1]
print(desired_output)

Q30. Resverse the string given in the above question.
ans:
string = "Big Data iNeuron"
desired_output = string[-1::-1] # reversing the string
print(desired_output)

Q31. How can you delete entire string at once?
ans: 
string ="Hello data"
del string # delete the entire string.

Q32. What is escape sequence?
ans:
\'	Single Quote	
\\	Backslash	
\n	New Line	
\r	Carriage Return	
\t	Tab	
\b	Backspace	
\f	Form Feed	


Q33. How can you print the below string?
```
'iNeuron's Big Data Course'
```
print("'iNeuron's Big Data Course'")

Q34. What is a list in Python?
ans:Lists are used to store multiple items in a single variable.Lists are one of 4 built-in data types in Python used to store collections of data, the other 3 are Tuple, Set, and Dictionary, all with different qualities and usage.

Q35. How can you create a list in Python?
ans: 
list = ["apple", "banana", "cherry"]

Q36. How can we access the elements in a list?
ans: we can use index to access the elements in the list.
thislist = ["apple", "banana", "cherry"]
print(thislist[0])
....apple
Q37. Write a code to access the word "iNeuron" from the given list.
```
lst = [1,2,3,"Hi",[45,54, "iNeuron"], "Big Data"]
``` 
ans: print(lst[4][2])
Q38. Take a list as an input from the user and find the length of the list.
ans: 
lst = input("Enter the element")
length_lst=len(lst) #length of element store in length_lst
print(length_lst)

Q39. Add the word "Big" in the 3rd index of the given list.
```
lst = ["Welcome", "to", "Data", "course"]
```
lst[3]="Big"
Q40. What is a tuple? How is it different from list?
ans:tuple is a index based data structure  we can acess data using [] the elements.tuple is use "()" parantesis.
One of the most important differences between list and tuple is that list is mutable, whereas a tuple is immutable. This means that lists can be changed, and tuples cannot be changed.

Q41. How can you create a tuple in Python?
ans:tuple = ('hello',23.56.5,"Hi")
Q42. Create a tuple and try to add your name in the tuple. Are you able to do it? Support your answer with reason.
ans: NO. tuple is immutable,it cannot change after created.
Q43. Can two tuple be appended. If yes, write a code for it. If not, why?
ans: yes, you can append two tuple and added in to new tuple as possible.
#initialize tuples
test_tup1 = (1, 3, 5)
test_tup2 = (4, 6)
#using + operator
res = test_tup1 + test_tup2
#printing result
print("The tuple after concatenation is : " + str(res))

Q44. Take a tuple as an input and print the count of elements in it.
ans:
values = input('Please enter some values:')
 #spliting the input values by space
input_tuple = tuple(int(val) for val in values.split())
print('tuple:',input_tuple)

Q45. What are sets in Python?
ans: set is a unordered and mutable collection of unique elements,set elements inside {}
eg:set_test = {12,45,7,8,89}

Q46. How can you create a set?
ans:set_test = {12,4,3,44,90}

Q47. Create a set and add "iNeuron" in your set.
ans :
new_set ={"good","morning","all"}
new_set.add("iNeuron")
Q48. Try to add multiple values using add() function.
ans:
add_multi_elements=set()
add_multi_elements.add("i'm")
add_multi_elements.add("learning")
add_multi_elements.add("python")
Q49. How is update() different from add()?
ans:Differences between add() and update() Use add() function to add a single element. Whereas use update() function to add multiple elements to the set.
Q50. What is clear() in sets?
ans:The clear () method removes all elements in a set.
Q51. What is frozen set?
ans:The frozenset () function returns an unchangeable frozenset object
Q52. How is frozen set different from set?
ans:Creation While you can create a set with the built-in set or through the {} notation, frozenset s can only be created through their respective built-in.Sets are mutable and frozen are not./

Q53. What is union() in sets? Explain via code.
ans: 
chocolates = {'munch','kitkat','diarymilk',"mango"}
fruits = {'mango','orange','pineapple',"munch"}
chocolates_fruits = chocolates.union(fruits)
print(chocolates_fruits)
output-->>> {'pineapple', 'mango', 'orange', 'kitkat', 'munch', 'diarymilk'}
 ''' the union will combine two sets and provide an distinct elements from both sets that means duplicate vales will be eliminate list will be the final result .

Q54. What is intersection() in sets? Explain via code.
ans: intersection() means the common elements from the tuple will be the output tuple.
eg: 
chocolates = {'munch','kitkat','diarymilk',"mango"}
fruits = {'mango','orange','pineapple',"munch"}
chocolates_fruits = chocolates.intersection(fruits)
print(chocolates_fruits)
output -->>> {'mango', 'munch'}

Q55. What is dictionary in Python?
ans:Dictionaries are used to store data values in key:value pairs.A dictionary is a collection which is ordered, changeable and do not allow duplicates.
Q56. How is dictionary different from all other data structures.
ans: other Data Types that hold only a single value as an element, Dictionary holds the key:value pair.
Q57. How can we delare a dictionary in Python?
ans:thisdict = {"brand": "Ford","model": "Mustang","year": 1964}

Q58. What will the output of the following?
```
var = {}
print(type(var))
```
ans: dict
Q59. How can we add an element in a dictionary?
ans:
new_dict={}
new_dict["Frist_name"]="krish"
new_dict["Last_name"]="na"
new_dict["age"]= 25

Q60. Create a dictionary and access all the values in that dictionary.
ans: 
# creating dictionary name as my_information
my_information = {'name': 'Dionysia' ,'age': 28,'location': 'Athens'}
values=my_information.values() # accessing values from the dictionary
print(values)
key=my_information.keys()      # accessing keys from the dictionary
print(key)
x=my_information.items()       # return elements in the dictionary as tuple inside list
print(x)

Q61. Create a nested dictionary and access all the element in the inner dictionary.
ans:
child1 = {"name" : "Emil","year" : 2004}
child2 = {"name" : "Tobias","year" : 2007}
child3 = {"name" : "Linus","year" : 2011 }

myfamily = {"child1" : child1,"child2" : child2,"child3" : child3}

for key,value in myfamily.items():
    print(f"key= {key}  and value = {value}" )

Q62. What is the use of get() function?
ans: get function is used to get value from dictionary
eg:
car = {"brand": "Ford","model": "Mustang","year": 1964}
x = car.get("model") #return the value of the key model
print(x)
output:-->> Mustang

Q63. What is the use of items() function?
ans: items function must Returns a list containing a tuple for each key value pair.

Q64. What is the use of pop() function?
ans: Removes the element with the specified key

Q65. What is the use of popitems() function?
ans:Removes the last inserted key-value pair

Q66. What is the use of keys() function?
ans: Returns a list containing the dictionary's keys

Q67. What is the use of values() function?
ans: Returns a list of all the values in the dictionary

Q68. What are loops in Python?
ans: Python has two premitive loop commands:
* for loop
*while loop

while loop :-while loop we can execute a set of statements as long as a condition is true.
eg:--Print i as long as i is less than 6:
i = 1
while i < 6:
  print(i)
  i += 1
for loop :- A for loop is used for iterating over a sequence (that is either a list, a tuple, a dictionary, a set, or a string).
eg:--Print each fruit in a fruit list:
fruits = ["apple", "banana", "cherry"]
for x in fruits:
  print(x)


Q69. How many type of loop are there in Python?
ans: 3 Types of loops in python.
*For loop using else statement
*The infinite Loop
*Nested loops

Q70. What is the difference between for and while loops?
ans:
*In a for loop, the set of declarations, including iterations and conditions, sits at the top of the body.
*In a while loop, initialization is always outside the loop. Before or after the execution of the statement(s), update can be performed.
*A for loop is a control flow statement that executes code repeatedly for a particular number of iterations.
*A loop that executes a single statement or a group of statements for the given true condition. The keyword used to represent this loop is while.
*When no condition is given in the for loop, the loop will iterate infinite times, while in the case of the while loop, it will give an error (compile time error).

Q71. What is the use of continue statement?
ans: Usage The continue keyword is used to end the current iteration in a for loop (or a while loop), and continues to the next iteration.

Q72. What is the use of break statement?
ans: Python break is used to terminate the execution of the loop.

Q73. What is the use of pass statement?
ans:The Python Pass statement is used as a placeholder within loops, functions, classes, and if-statements that will be implemented later.
In Python, a Pass statement is a null statement that is used in cases where the loop, function, or class is to be ignored or written and executed in the future.

Q74. What is the use of range() function?
ans:The range function in Python aids in the generation of numerical sequences.Python range is a built-in function that returns a sequence of numbers based on the start and finishes index provided

Q75. How can you loop over a dictionary?
ans: we can loop threw dictionary using for loop.
thisdict ={"name":'krish',"age":24,"Nationality":"indian","year"=2022}
#Print all key names in the dictionary, one by one:
for x in thisdict:
  print(x)

#Print all values in the dictionary, one by one:
for x in thisdict:
  print(thisdict[x])

#You can also use the values() function to return values of a dictionary:
for x in thisdict.values():
  print(x)

#Loop through both keys and values, by using the items() function:
for x, y in thisdict.items():
  print(x, y)

### Coding problems
Q76. Write a Python program to find the factorial of a given number.
ans: 
def fact(n): #function to find the factorial and return the factorial.
    mul=1
    for num in range(1,n+1):
        mul *=num
    return mul

factorial = fact(5)
print(factorial)

Q77. Write a Python program to calculate the simple interest. Formula to calculate simple interest is SI = (P*R*T)/100
ans:
P,R,T=20,10,40
Si =(P*R*T)/100
print("simple interst = ",Si)

Q78. Write a Python program to calculate the compound interest. Formula of compound interest is A = P(1+ R/100)^t.
ans: 
 inputs
p= 1200   # principle amount
t= 2      # time
r= 5.4    # rate
#calculates the compound interest
a=p*(1+(r/100))**t 
print("The compound interest is "a)
Q79. Write a Python program to check if a number is prime or not.
ans:
number = int(input("Enter any number:"))
if number>1:
    for i in range(2,number):
        if (number%i)==0:
            print(number, "is not prime number")
            break
    else:
            print(number, "is prime number")

Q80. Write a Python program to check Armstrong Number.
ans:
#take input from the user
num = int(input("Enter a number: "))
#initialize sum
sum = 0
#find the sum of the cube of each digit
temp = num
while temp > 0:
   digit = temp % 10
   sum += digit ** 3
   temp //= 10
#display the result
if num == sum:
   print(num,"is an Armstrong number")
else:
   print(num,"is not an Armstrong number")

Q81. Write a Python program to find the n-th Fibonacci Number.
ans:
def Fibonacci(n):
	if n<= 0:
		print("Incorrect input")
	elif n == 1:
		return 0
	elif n == 2:
		return 1
	else:
		return Fibonacci(n-1)+Fibonacci(n-2)
print(Fibonacci(10))

Q82. Write a Python program to interchange the first and last element in a list.
ans:
#list
lst = [23, 100, 54, 56, 98]
#interchanging the first and last element
lst[0], lst[-1] = lst[-1], lst[0]
print(lst)

Q83. Write a Python program to swap two elements in a list.
ans:
#creating a function  
def swap_pos(lst, a, b):  
#popping the elements from list      
    f_ele=lst.pop(a)  
    s_ele=lst.pop(b-1)  
#inserting in the respective positions      
    lst.insert(a, s_ele)  
    lst.insert(b, f_ele)  
    return lst  
#initialising the list  
lst_val=[20, 13, 41, 11, 10, 29]  
#displaying the original list  
print("The values inside the list are: ", lst_val)  
#specifying the positions  
a, b=2, 5  
#passing the values in function  
print("The list with swapped elements is: ", swap_pos(lst_val,a-1,b-1))

Q84. Write a Python program to find N largest element from a list.
ans:
def Nmaxelements(list1, N):
	final_list = []

	for i in range(0, N):
		max1 = 0
		
		for j in range(len(list1)):	
			if list1[j] > max1:
				max1 = list1[j];
				
		list1.remove(max1);
		final_list.append(max1)
		
	print(f"{N}th largest number is ",final_list[-1])

list1 = [2, 6, 41, 85, 0, 3, 7, 6, 10]
N = int(input("enter the nth value"))

#Calling the function
Nmaxelements(list1, N)

Q85. Write a Python program to find cumulative sum of a list.
ans:
given_list = [34, 45, 12, 22, 33, 75, 10, 98, 222, 999, 1023, 32421]
countsum = 0
#empty list say cumulativelist which stores the cumulative sum.
cumulativelist = []
length = len(given_list)
for i in range(length):
    countsum = countsum+given_list[i]
    cumulativelist.append(countsum)
print("The given list before calculating cumulative sum ", given_list)

print("The given list before calculating cumulative sum ", cumulativelist)

Q86. Write a Python program to check if a string is palindrome or not.
ans:
#function which return reverse of a string

def isPalindrome(s):
	return s == s[::-1]

s = "malayalam"
ans = isPalindrome(s)

if ans:
	print(f"{s} is palindrome")
else:
	print(f"{s} is not a palindrome")


Q87. Write a Python program to remove i'th element from a string.
ans:
test_str = "GeeksForGeeks"
new_str = ""

print("The string : ",test_str)
Pos =int (input("Enter the position of element "))
if Pos > len(test_str):
    print("please check the postion !!!")
else:
    for i in range(len(test_str)):
        if i != Pos-1:
            new_str = new_str + test_str[i]
print ("The string after removal of i'th character : " + new_str)

Q88. Write a Python program to check if a substring is present in a given string.
ans:

MyString1 = "iNeuron is a online platform giving training"

if "online" in MyString1:
	print("Yes! it is present in the string")
else:
	print("No! it is not present")

Q89. Write a Python program to find words which are greater than given length k.
ans:
def string_k(k, str):
	# create the empty string
	string = []
	# split the string where space is comes
	text = str.split(" ")	
	# iterate the loop till every substring
	for x in text:
		if len(x) > k:
			string.append(x)
	return string	
k = 3
str ="iNeuron big data "
print(string_k(k, str))
Q90. Write a Python program to extract unique dictionary values.
ans:
#initializing dictionary
test_dict = {'gfg' : [5, 6, 7, 8],'is' : [10, 11, 7, 5],'best' : [6, 12, 10, 8],'for' : [1, 2, 5]}

#printing original dictionary
print("The original dictionary is : " + str(test_dict))

#Extract Unique values dictionary values
x=[]
for i in test_dict.keys():
	x.extend(test_dict[i])
x=list(set(x))
x.sort()
print("The unique values list is : " + str(x))

Q91. Write a Python program to merge two dictionary.
ans:
dict1 = {  'Rahul': 4, 'Ram': 9, 'Jayant' : 10 }
dict2 = {  'Jonas': 4, 'Niel': 9, 'Patel' : 10 }
 
dict1.update(dict2)
print("after updating :")
print(dict1)

Q92. Write a Python program to convert a list of tuples into dictionary.
```
Input : [('Sachin', 10), ('MSD', 7), ('Kohli', 18), ('Rohit', 45)]
Output : {'Sachin': 10, 'MSD': 7, 'Kohli': 18, 'Rohit': 45}
```
ans: print((dict([('Sachin', 10), ('MSD', 7), ('Kohli', 18), ('Rohit', 45)])))

Q93. Write a Python program to create a list of tuples from given list having number and its cube in each tuple.
```
Input: list = [9, 5, 6]
Output: [(9, 729), (5, 125), (6, 216)]
```
ans:Method --1
list = [9, 5, 6] 
output = [(val, val**3) for val in list] # using list comperhension
print(output)

method --2
list = [9, 5, 6] 
res = []
for i in range(len(list)):
    res.append((list[i],list[i]**3))
print(res)
Q94. Write a Python program to get all combinations of 2 tuples.
```
Input : test_tuple1 = (7, 2), test_tuple2 = (7, 8)
Output : [(7, 7), (7, 8), (2, 7), (2, 8), (7, 7), (7, 2), (8, 7), (8, 2)]
```
ans:
test_tuple1 = (7, 2)
test_tuple2 = (7, 8)
print("First tuple : " + str(test_tuple1))
print("Second tuple : " + str(test_tuple2))
#finding all pair Combination of tuples 
pairComb = [] 
for val1 in test_tuple1:
    for val2 in test_tuple2:
        tup = [val1, val2]
        pairComb.append(tuple(tup))

for val1 in test_tuple2:
    for val2 in test_tuple1:
        tup = [val1, val2]
        pairComb.append(tuple(tup))
print("All pair Combinations are  : " + str(pairComb))

Q95. Write a Python program to sort a list of tuples by second item.
```
Input : [('for', 24), ('Geeks', 8), ('Geeks', 30)] 
Output : [('Geeks', 8), ('for', 24), ('Geeks', 30)]
```
ans:
def Sort_Tuple(tup):
	tup.sort(key = lambda x: x[1])
	return tup

tup = [('for', 24), ('Geeks', 8), ('Geeks', 30)]
print(Sort_Tuple(tup))
Q96. Write a python program to print below pattern.
```
* 
* * 
* * * 
* * * * 
* * * * * 
```
ans:
length=int(input("Enter the no of rows: " ))
for row in range(length+1):
    print('* '*row)

Q97. Write a python program to print below pattern.
```
    *
   **
  ***
 ****
*****
```
ans:
row =int(input("Enter the no of rows: "))
for i in range(row+1):
	for space in range(i,row):
		print(' ',end=" ")
	for j in range(i):
		print('*',end=' ')
	print()

Q98. Write a python program to print below pattern.
```
    * 
   * * 
  * * * 
 * * * * 
* * * * * 
```
ans:
row =int(input("Enter the no of rows: "))
for i in range(row+1):
	for space in range(i,row):
		print('',end=" ")
	for column in range(i):
		print('*',end='  ')
	print()

Q99. Write a python program to print below pattern.
```
1 
1 2 
1 2 3 
1 2 3 4 
1 2 3 4 5
```
ans:
row =5
for i in range(row+1):
	for column in range(1,i+1):
		print(column,end=" ")
	print()


Q100. Write a python program to print below pattern.
```
A 
B B 
C C C 
D D D D 
E E E E E 
```
ans:
row =5  #no of rows
for i in range(row):
	for j in range(i+1):
		print(chr(i+65),end=" ")  #ASCII value 65 = 'A'
	print()
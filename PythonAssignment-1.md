## Assignment Part-1
Q1. Why do we call Python as a general purpose and high-level programming language?

In computer software, a general-purpose programming language (GPL) is a programming language designed to be used for building software in a wide     variety of application domains, across a multitude of hardware configurations and operating systems.
Python is considered as a high level programming language because they are not written in machine-readable language, Python programs need to be processed before machines can run them. Python is an interpreted language. This means that every time a program is run, its interpreter runs through the code and translates it into machine-readable byte code.

Q2. Why is Python called a dynamically typed language?

Python don't have any problem even if we don't declare the type of variable. Dynamic typing means that the type of the variable is determined only during runtime. Python also take cares of the memory management which is crucial in programming. So, Python is a dynamically typed language.

Q3. List some pros and cons of Python programming language?


              Pros                                                 Cons
         Beginner-friendly	                                  Issues with design
          Large Community	                             Slower than compiled languages
       Flexible and Extensible                                   Security
       Extensive Libraries	                                  Work Environment
           Embeddable	                                   High memory consumption
         Highly Scalable	                                  Dynamically-typed language
        IoT Opportunities	                                Complex multithreading
          Portable	                             Garbage collection leads to potential memory losses

Q4. In what all domains can we use Python?

 Data Science, Automation, Application Development, AI & Machine Learning, Audio/Video application, Console application

Q5. What are variable and how can we declare them?

Python is a dynamic-typed language, which means we don't need to mention the variable type or declare before using it. It makes to Python the most efficient and easy to use language. Every variable is treated as an object in Python.

num = 25                                           str_var = 'JavaTpoint'  
print("The type of a", type(num))                  print(str_var)  
print(num)                                         print(type(str_var))  

Q6. How can we take an input from the user in Python?

name = input("Enter your name: ")                  # String Input  
age = int(input("Enter your age: "))               # Integer Input  
marks = float(input("Enter your marks: "))         # Float Input  

By default, the input() function takes input as a string so if we need to enter the integer or float type input then the input() function must be type casted.

Q7. What is the default datatype of the value that has been taken as an input using input() function?

By default, the input() function takes input as a string so if we need to enter the integer or float type input then the input() function must be type casted.

Q8. What is type casting?

Type Casting is the method to convert the variable data type into a certain data type in order to the operation required to be performed by users.

Q9. Can we take more than one input from the user using single input() function? If yes, how? If no, why?

# taking two inputs at a time  
a, b, c = input("Enter three values: ").split()  
print("Enter Your First Name: ", a)  
print("Enter Your Last Name: ", b)  
print("Enter Your Class: ", c)  
print()  

Enter three values: David Warner MCA
Enter Your First Name:  David
Enter Your Last Name:  Warner
Enter Your Class:  Warner

Q10. What are keywords?

Keywords in Python are unique reserved words. We that cannot use a keyword as a variable, function, or other identifiers. These special words are used to define the syntax and structure of the Python language.

Q11. Can we use keywords as a variable? Support your answer with reason.

No, keywords are some predefined and reserved words in python that have special meanings. Keywords are used to define the syntax of the coding.

Q12. What is indentation? What's the use of indentaion in Python?

Indentation refers to the spaces at the beginning of a code line. Where in other programming languages the indentation in code is for readability only, the indentation in Python is very important. Python uses indentation to indicate a block of code.

Q13. How can we throw some output in Python?

Python print() function prints the message to the screen or any other standard output device.

Q14. What are operators in Python?

In Python, operators are special symbols that designate that some sort of computation should be performed. The values that an operator acts on are called operands. 
Here is an example: >>> >>> a = 10 >>> b = 20 >>> a + b 30. 
In this case, the + operator adds the operands a and b together.

Q15. What is difference between / and // operators?

'/' is the division operator.     '//' is the floor division operator.

a = 19  b = 4
print(a // b)  #This prints output as 4   
print(a / b)  #This prints output as 4.75

Q16. Write a code that gives following as an output.
```
iNeuroniNeuroniNeuroniNeuron
```

Print("iNeuroniNeuroniNeuroniNeuron")

Q17. Write a code to take a number as an input from the user and check if the number is odd or even.

num = int(input("Enter Name: "))
if(num%2==0):
    print("Number is even")
else:
    print("Number is odd")


Q18. What are boolean operator?

Boolean Operators are simple words (AND, OR, NOT or AND NOT) used as conjunctions to combine or exclude keywords in a search, resulting in more focused and productive results

Q19. What will the output of the following?
```
1 or 0                              1

0 and 0                             0

True and False and True              False

1 or 0 or 0                          1
```

Q20. What are conditional statements in Python?

A conditional statement as the name suggests itself, is used to handle conditions in your program. We have different types of conditional statements like if, if-else, elif, nested if, and nested if-else statements which control the execution of our program.

Q21. What is use of 'if', 'elif' and 'else' keywords?

if… elif…else are conditional statements that provide you with the decision making that is required when you want to execute code based on a particular condition. The if… elif…else statement used in Python helps automate that decision making process.

Q22. Write a code to take the age of person as an input and if age >= 18 display "I can vote". If age is < 18 display "I can't vote".

age = int(input("Enter age: "))
if(age>=18):
  print("I can vote")
else:
  print("I cannot vote")

Q23. Write a code that displays the sum of all the even numbers from the given list.
```
numbers = [12, 75, 150, 180, 145, 525, 50]
```
list_sum = 0
for num in numbers:
  if num%2 == 0:
   list_sum = list_sum + num
print(list_sum)

Output -> 392

Q24. Write a code to take 3 numbers as an input from the user and display the greatest no as output.

a = int(input('Enter first number  : '))
b = int(input('Enter second number : '))
c = int(input('Enter third number  : '))

largest = 0

if a > b and a > c:
    largest = a
if b > a and b > c:
    largest = b
if c > a and c > b:
    largest = c

print(largest, "is the largest of three numbers.")

Q25. Write a program to display only those numbers from a list that satisfy the following conditions

- The number must be divisible by five

- If the number is greater than 150, then skip it and move to the next number

- If the number is greater than 500, then stop the loop
```
numbers = [12, 75, 150, 180, 145, 525, 50]
```

numbers = [12, 75, 150, 180, 145, 525, 50]

for i in numbers:
    if i%5==0:
        if i > 150 and i <=500:
            continue
        elif i > 500:
            break
        else:
            print(i)
Q26. What is a string? How can we declare string in Python?

Ans26. In Python, Strings are arrays of bytes representing Unicode characters.

Q27. How can we access the string using its index?

Ans27. Sqaure brackets can used to access the elements of the string.

Q28. Write a code to get the desired output of the following

string = "Big Data iNeuron"
desired_output = "iNeuron"

Ans28.
string[9:16]

Q29. Write a code to get the desired output of the following

string = "Big Data iNeuron"
desired_output = "norueNi"

Ans29.
string[15:8:-1]

Q30. Resverse the string given in the above question. 

Ans30.
string[::-1]

Q31. How can you delete entire string at once?

Ans31. We can delete the entire string at once by using del keyword.

str1 = "Hello"
del(str1)

Q32. What is escape sequence?

Ans32. The "backslash ()" character as an escape character. In other words, it has a special meaning when we use it inside the strings. As the name suggests, the escape character escapes the characters in a string for a brief moment to introduce unique inclusion.

Q33. How can you print the below string?

'iNeuron's Big Data Course'

Ans33. print("'iNeuron's Big Data Course'")

Q34. What is a list in Python?

Ans34. Python list are dynamically sized array, declared in languages like C++ and Java. A list is a collection of things, enclosed in [ ] and separated by commas.

Q35. How can you create a list in Python?

Ans35. You can create a list by opening and closing the square brackets.

Q36. How can we access the elements in a list?

Ans36. We can access the elements in a list by indexing.

Q37. Write a code to access the word "iNeuron" from the given list.

lst = [1,2,3,"Hi",[45,54, "iNeuron"], "Big Data"]

Ans37.

lst[4][2]

Q38. Take a list as an input from the user and find the length of the list.

Ans38.

n = input("Enter number of elements seprated by space: ").split(" ")
print(len(n))

Q39. Add the word "Big" in the 3rd index of the given list.

lst = ["Welcome", "to", "Data", "course"]
Ans39.

lst.insert(2, "Big")

Q40. What is a tuple? How is it different from list?

Ans40. Tuple is a collection of Python objects much like a list. The sequence of values stored in a tuple can be of any type, and they are indexed by integers. Tuples are immutable where as list are mutable. We can also faster through the tuples than the list.

Q41. How can you create a tuple in Python?

Ans41. We can create tuple using round brackets ().

Q42. Create a tuple and try to add your name in the tuple. Are you able to do it? Support your answer with reason.

Ans42. No, I can't as tuples are immutable. The work around is it typecast tuple to list and then append.

tup = ()
tup = list(tup)    //typecasting
tup.append("raj")
print(tup)

Q43. Can two tuple be appended. If yes, write a code for it. If not, why?

Ans43.Yes, we can.

tup1 = ("Vishal ")
tup2 = ("Singh")
print(tup1+tup2)

Q44. Take a tuple as an input and print the count of elements in it.

Ans44.

x = input("Enter the values separeted by space: ").split(" ")
x = tuple(x)
print(len(x))

Q45. What are sets in Python?

Ans45. A set is an unordered collection of data types that is iterable, mutable and has no duplicate elements. The order of elements in a set is undefined though it may consist of various elements.

Q46. How can you create a set?

Ans46. We can create set using curly brackets {}. Keep in mind empty {} will result in dictionary hence there must be some value in the brackets.

Q47. Create a set and add "iNeuron" in your set.

Ans47.

set1 = {"iNeuron"}
print(set1)

Q48. Try to add multiple values using add() function.

Ans48.

set1.add("Big")
set1.add("Data")
print(set1)

Q49. How is update() different from add()?

Ans49. We can add more than one element in a single go using update(), but using add() it's not possible.

Q50. What is clear() in sets?

Ans50. To remove all the elements from the set, clear() function is used.

Q51. What is frozen set?

Ans51. Frozen sets in Python are immutable objects that only support methods and operators that produce a result without affecting the frozen set or sets to which they are applied. While elements of a set can be modified at any time, elements of the frozen set remain the same after creation.

Q52. How is frozen set different from set?

Ans52.
Frozen sets are immutable where as sets are mutable.
Sets can't be used as keys in dictionary where as frozen sets can be used.

Q53. What is union() in sets? Explain via code.

Ans53. Python set Union() Method returns a new set which contains all the items from the original set.

set1 = {2, 4, 5, 6}
set2 = {4, 6, 7, 8}
set3 = {7, 8, 9, 10}

print("set1 U set2 : ", set1 | set2)

print("set1 U set2 U set3 :", set1 |set2 | set3)

Q54. What is intersection() in sets? Explain via code.

Ans54. Python set intersection() method returns a new set with an element that is common to all set

set1 = {2, 4, 5, 6}
set2 = {4, 6, 7, 8}
set3 = {4, 6, 8}

print("set1 intersection set2 : ", set1.intersection(set2))

print("set1 intersection set2 intersection set3 :", set1.intersection(set2, set3))

Q55. What is dictionary in Python?

Ans55. Dictionary in Python is a collection of keys values, used to store data values like a map, which, unlike other data types which hold only a single value as an element.

Q56. How is dictionary different from all other data structures.

Ans56. Dictionary is having key and value pair where as all other data structures have only values in them.

Q57. How can we delcare a dictionary in Python?

Ans57. We can create dictionary using curly brackets {}.

Q58. What will the output of the following?

var = {}
print(type(var))

Ans58. dict

Q59. How can we add an element in a dictionary?

Ans59.

Dict = {}
Dict[0] = "Hello"
Dict[1] = "Course: ["Data Science", "Big Data"]"

Q60. Create a dictionary and access all the values in that dictionary.

Ans60.

Dict = {"Name": "Vishal", "Experience": 3, "Organisation":"iNeuron"}
for i, j in Dict.items():
  print("Key is ",i, "and value is ",j)

Q61. Create a nested dictionary and access all the element in the inner dictionary.

Ans61.

Dict = {"Name": {"f_name":"Vishal", "l_name":"Singh"}, "Experience": 3, "Organisation":"iNeuron"}
for i, j in Dict["Name"].items():
  print(f"Key is {i} and value is {j}")
  
Q62. What is the use of get() function?

Ans62. get() is also to access the elements in dictionary.

Dict = {"Name": "Vishal", "Experience": 3, "Organisation":"iNeuron"}
print(Dict.get("Name"))

Q63. What is the use of items() function?

Ans63. items() method is used to return the list with all dictionary keys with values.

Dict = {"Name": "Vishal", "Experience": 3, "Organisation":"iNeuron"}
print(Dict.items())

Output - dict_items([('Name', 'Vishal'), ('Experience', 3), ('Organisation', 'iNeuron')])

Q64. What is the use of pop() function?

Ans64.

Dict = {"Name": "Vishal", "Experience": 3, "Organisation":"iNeuron"}
print(Dict.pop("Name"))

output - Vishal

Q65. What is the use of popitems() function?

Ans65. popitem() method removes the last inserted key-value pair from the dictionary and returns it as a tuple.

Dict = {"Name": "Vishal", "Experience": 3, "Organisation":"iNeuron"}
print(Dict.popitem())

Output - ('Organisation', 'iNeuron')

Q66. What is the use of keys() function?

Ans66. keys() method returns a view object that displays a list of all the keys in the dictionary.

Dict = {"Name": "Vishal", "Experience": 3, "Organisation":"iNeuron"}
print(Dict.keys())

Output - dict_keys(['Name', 'Experience', 'Organisation'])

Q67. What is the use of values() function?

Ans67. values() is an inbuilt method in Python programming language that returns a view object. The view object contains the values of the dictionary, as a list.

Dict = {"Name": "Vishal", "Experience": 3, "Organisation":"iNeuron"}
print(Dict.values())

Output - dict_values(['Vishal', 3, 'iNeuron'])

Q68. What are loops in Python?

Ans68. Loops are used the iterate over a block of statement multiple times.

Q69. How many type of loop are there in Python?

Ans69. There is for and while loop in Python

Q70. What is the difference between for and while loops?

Ans70. When we know the exact number of iterations, we can use for loop. When we want the to run till a certain condition is true we can use while loop.

Q71. What is the use of continue statement?

Ans71. Continue Statement skips the execution of the program block from after the continue statement and forces the control to start the next iteration.

Q72. What is the use of break statement?

Ans72. break statement in Python is used to bring the control out of the loop when some external condition is triggered. break statement is put inside the loop body

Q73. What is the use of pass statement?

Ans73. The pass statement is a null statement. But the difference between pass and comment is that comment is ignored by the interpreter whereas pass is not ignored.

Q74. What is the use of range() function?

Ans74. range() function returns a sequence of numbers, in a given range. The most common use of it is to iterate sequence on a sequence of numbers
  
Q75. How can you loop over a dictionary?

Ans75.  
statesAndCapitals = {
	'Gujarat': 'Gandhinagar',
	'Maharashtra': 'Mumbai',
	'Rajasthan': 'Jaipur',
	'Bihar': 'Patna'
}

for state,city in statesAndCapitals.items():
	print(state,"=",city)

Coding problems
Q76. Write a Python program to find the factorial of a given number.

Ans76.

def factorial(n):
  if n < 0:
    return 0
  elif n == 0 or n == 1:
    return 1
  else:
    fact = 1
    while(n>1):
      fact = fact* n
      n = n-1
    return fact

n=6
output = factorial(n)
print("Factorial =",output)

Q77. Write a Python program to calculate the simple interest. Formula to calculate simple interest is SI = (PRT)/100

Ans77.

def SI(p,r,t):
  si = (p*r*t)/100
  
  return si

output = SI(8, 8, 6)
print("Simple interest is ",output)

Q78. Write a Python program to calculate the compound interest. Formula of compound interest is A = P(1+ R/100)^t.

Ans78.

def CI(p, r, t):
  amount = p*(1+r/100)**t
  ci = amount - p
  return ci

output = CI(10000, 10.25, 5)
print(f"Compound intrest is ",output)

Q79. Write a Python program to check if a number is prime or not.

Ans79.

def is_prime(n):
    flag =False
    if(n==1 & n==0):
        print("it is not a prime number ")
    elif(n>1):
        for i in range(2,n):
            if n%i==0:
                flag = True
                break
        if flag:
           print(n,"It is not a prime number")
        else:
           print(n, "It is a prime number")            
    
num = int(input("Enter a number: "))
is_prime(num)

Q80. Write a Python program to check Armstrong Number.

Ans80.

def check_armstrong(n):
  s = n
  b = len(str(n))
  sum1 = 0
  while n != 0:
      r = n % 10
      sum1 = sum1+(r**b)
      n = n//10
  if s == sum1:
      print(f"The given number {s} is armstrong number")
  else:
      print(f"The given number {s} is not armstrong number")

check_armstrong(153)
    
Q81. Write a Python program to find the n-th Fibonacci Number.

Ans81.

def Fibonacci(n):
	if n<= 0:
		print("Incorrect input")
	elif n == 1:
		return 0
	elif n == 2:
		return 1
	else:
		return Fibonacci(n-1)+Fibonacci(n-2)

print(Fibonacci(7))
 
Q82. Write a Python program to interchange the first and last element in a list.

Ans82.

def swap_list(newList):
	size = len(newList)
	temp = newList[0]
	newList[0] = newList[size - 1]
	newList[size - 1] = temp
	
	return newList

newList = [15, 12, 35, 17, 9, 56, 29]

Q83. Write a Python program to swap two elements in a list.

Ans83.

def swapPositions(list, pos1, pos2):
	
	list[pos1], list[pos2] = list[pos2], list[pos1]
	return list

List = [15, 12, 35, 17, 9, 56, 29]
pos1, pos2 = 1, 3

Q84. Write a Python program to find N largest element from a list.

Ans84.

def n_max_elements(list1, N):
	final_list = []

	for i in range(0, N):
		max1 = 0
		
		for j in range(len(list1)):	
			if list1[j] > max1:
				max1 = list1[j];
				
		list1.remove(max1);
		final_list.append(max1)
		
	print(final_list)

list1 = [2, 6, 41, 85, 0, 3, 7, 6, 10]
N = 3

n_max_elements(list1, N)

Q85. Write a Python program to find cumulative sum of a list.

Ans85.

def cumulative_sum(lists):
	cu_list = []
	length = len(lists)
	cu_list = [sum(lists[0:x:1]) for x in range(0, length+1)]
	return cu_list[1:]

lists = [10, 20, 30, 40, 50]
print(f"Cumulative sum of the list is {cumulative_sum(lists)}")

Q86. Write a Python program to check if a string is palindrome or not.

Ans86.

def isPalindrome(s):
  if s == s[::-1]:
	  return f"{s} is palindrome"
  return f"{s} is not palindrome"

s = "dad"
isPalindrome(s)
Q87. Write a Python program to remove i'th element from a string.

Ans87.

def remove_ith_element(i):
  str1 = "Big Data Bootcamp"
  str2 = ""

  for n in range(len(str1)):
    if n == i:
      continue
    else:
      str2 = str2 + str1[n]

  print(str2)

remove_ith_element(5)

Q88. Write a Python program to check if a substring is present in a given string.

Ans88.

def check_substring(s2, s1):
	if (s2.count(s1) > 0):
		print(f'"{s1}" is a substring of "{s2}"')
	else:
		print(f'"{s1}" is not a substring of "{s2}"')


s2 = "Welcome to iNeuron Big Data Bootcamp"
s1 = "iNeuron"
check_substring(s2, s1)


Q89. Write a Python program to find words which are greater than given length k.

Ans89.

def string_greater_than_k(k, str):
	
	string = []

	text = str.split(" ")

	for x in text:

		if len(x) > k:

			string.append(x)

	return string

k = 3
str ="Big Data Bootcamp"
print(string_greater_than_k(k, str))

Output - ['Data', 'Bootcamp']

Q90. Write a Python program to extract unquire dictionary values.

Ans90.

test_dict = {'iNeuron': [5, 6, 7, 8],
			'is': [10, 11, 7, 5],
			'best': [6, 12, 10, 8],
			'for': [1, 2, 5],
      'big data': [2, 7, 12, 9]
      }

print("The original dictionary is : " + str(test_dict))

res = list(sorted({ele for val in test_dict.values() for ele in val}))

print("The unique values list is : " + str(res))

Output - The original dictionary is : {'iNeuron': [5, 6, 7, 8], 'is': [10, 11, 7, 5], 'best': [6, 12, 10, 8], 'for': [1, 2, 5], 'big data': [2, 7, 12, 9]}
The unique values list is : [1, 2, 5, 6, 7, 8, 9, 10, 11, 12]

Q91. Write a Python program to merge two dictionary.

Ans91.

def Merge(dict1, dict2):
	return(dict2.update(dict1))

dict1 = {'a': 10, 'b': 8}
dict2 = {'d': 6, 'c': 4}

print(Merge(dict1, dict2))

print(dict2)

Q92. Write a Python program to convert a list of tuples into dictionary.

Input : [('Sachin', 10), ('MSD', 7), ('Kohli', 18), ('Rohit', 45)]
Output : {'Sachin': 10, 'MSD': 7, 'Kohli': 18, 'Rohit': 45}

Ans92.

print (dict([('Sachin', 10), ('MSD', 7), ('Kohli', 18), ('Rohit', 45)]))

Q93. Write a Python program to create a list of tuples from given list having number and its cube in each tuple.

Input: list = [9, 5, 6]
Output: [(9, 729), (5, 125), (6, 216)]

Ans93.

list1 = [9, 5, 6]

res = [(val, pow(val, 3)) for val in list1]

print(res)

Q94. Write a Python program to get all combinations of 2 tuples.

Input : test_tuple1 = (7, 2), test_tuple2 = (7, 8)
Output : [(7, 7), (7, 8), (2, 7), (2, 8), (7, 7), (7, 2), (8, 7), (8, 2)]
Ans94.

test_tuple1 = (7, 2)
test_tuple2 = (7, 8)

res = [(a, b) for a in test_tuple1 for b in test_tuple2]
res = res + [(a, b) for a in test_tuple2 for b in test_tuple1]

print("The filtered tuple : ", str(res))

Q95. Write a Python program to sort a list of tuples by second item.

Input : [('452', 10), ('256', 5), ('100', 20), ('135', 15)]
Output : [('256', 5), ('452', 10), ('135', 15), ('100', 20)]
Ans95.

def Sort_Tuple(tup):
     
    lst = len(tup)
    for i in range(0, lst):
         
        for j in range(0, lst-i-1):
            if (tup[j][1] > tup[j + 1][1]):
                temp = tup[j]
                tup[j]= tup[j + 1]
                tup[j + 1]= temp
    return tup
 
tup =[('452', 10), ('256', 5), ('100', 20), ('135', 15)]
       
print(Sort_Tuple(tup))

Q96. Write a python program to print below pattern.

* 
* * 
* * * 
* * * * 
* * * * * 

Ans96.

def pypart(n):
	
	for i in range(0, n):
	
		for j in range(0, i+1):
		
			print("* ",end="")
	
		print("\r")

n = 5
pypart(n)

Q97. Write a python program to print below pattern.

    *
   **
  ***
 ****
*****

Ans97.

def inverse_pattern():
  n=5;i=0
  while(i<=n):
    print(" " * (n - i) +"*" * i)
    i+=1

inverse_pattern()

Q98. Write a python program to print below pattern.

    * 
   * * 
  * * * 
 * * * * 
* * * * * 

Ans98.

def triangle(n):
	
	k = n - 1

	for i in range(0, n):

		for j in range(0, k):
			print(end=" ")
	
		k = k - 1
	
		for j in range(0, i+1):

			print("* ", end="")
	
		print("\r")

n = 5
triangle(n)

Q99. Write a python program to print below pattern.

1 
1 2 
1 2 3 
1 2 3 4 
1 2 3 4 5

Ans99.

def numpat(n):

	num = 1

	for i in range(0, n):

		num = 1

		for j in range(0, i+1):

			print(num, end=" ")

			num = num + 1

		print("\r")

n = 5
numpat(n)

Q100. Write a python program to print below pattern.

A 
B B 
C C C 
D D D D 
E E E E E 
Ans100.

def alphapat(n):

	num = 65

	for i in range(0, n):
	
		for j in range(0, i+1):

			ch = chr(num)
		
			print(ch, end=" ")
	
		num = num + 1
	
		print("\r")

n = 5
alphapat(n)













            

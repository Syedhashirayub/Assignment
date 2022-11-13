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
            
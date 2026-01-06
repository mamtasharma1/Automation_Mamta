# Automation_Mamta#Python#Calculator

# python program to create a simple calculator
#WAP to create a calculator that can perform at least five diff mathematical operations such as :
#add,sub,multi,div and avg
#prompting for input and displaying the results clearly
#Defining functions :
def add(a,b):
    return a+b
def sub(a,b):
    return a-b
def mul(a,b):
    return a*b
def div(a,b):
    return a/b
def avg(a,b):
    return (a+b)/2
#user input
print("Please select an operation :\n"\
      "1.Addition \n"\
      "2.Substraction \n"\
      "3.Multiplication \n"\
      "4.Division \n"\
      "5.Average \n" )
select = int(input("select an option from 1,2,3,4,5:"))
number1 = int(input("Enter first number : "))
number2 = int(input("Enter second number: "))

#print the result
if(select == 1):
    print (number1,"+" , number2,"=",\
           add(number1,number2))
elif(select == 2):
    print (number1,"-" , number2,"=",\
           sub(number1,number2)) 
elif(select == 3):
    print (number1,"*" , number2,"=",\
           mul(number1,number2))  
elif(select == 4):
    print (number1,"/" , number2,"=",\
           div(number1,number2))
elif(select == 5):
    print("(",number1, "+", number2, ")", "/", "2", "= ", \
           avg(number1, number2))
else:
    print("Invalid option,please select again!")


COMMAND LINE ARGUMENTS:
--------------------------
Command-line arguments are values you pass to a program when you run it from the terminal/command prompt, instead of typing input during execution.
Python reads command-line arguments using the "sys" module.

EXAMPLE:
---------

import sys

def add(num1, num2):
    add = num1 + num2
    return add
def sub(num1, num2):
    sub = num1 - num2
    return sub
def mul(num1, num2):
    mul = num1 * num2
    return mul

num1 = float(sys.argv[1])  # First value which we pass in command
operation = sys.argv[2] # Second value which we pass in command
num2 = float(sys.argv[3]) # Third value which we pass in command

if operation == "add":
    output = add(num1, num2)
    print(output)
	
RESULT: python cmdLA.py 10 add 2
-----------------------------------
12.0


ENVIRONMENT VARIABLES:
------------------------
In python we can use OS environment variables to store and call sensitive data like password,token,keys and what evere we feel sensitive.
This can be use by importing "os" module in .py file.

We need set environment variable in our os first then call them in py file.

root@:~/python# export password="pythonsandeep"
root@:~/python# env | grep password
password=pythonsandeep


EXAMPLE: environmentvar.py
---------------------------
import os
print(os.getenv("password"))

RESULT:python environmentVAR.py
--------------------------------
pythonsandeep


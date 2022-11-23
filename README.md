# ProgrammingAssignment330

## Describes what the program does:
Think of simulating a security installation very similar to those installed in many offices and homes. The installation has a keypad and an engine (a controller) used to decide whether the user has entered the correct access code or not.

The keypad has ten keys, labeled from '0' to '9'. The security engine will unlock the lock when it finds the correct un-locking access code in the input string. Likewise, the security engine will lock the lock when it finds the correct locking access code in the input string.

DDDDD1 is the unlocking code
DDDDD4 is the locking code, where DDDDD are the lest significant five digits in your student ID. (59823)
As soon as the last digit of the access code is entered, your program will signal the action taken (lock or unlock).

## How to build and run the executable:
To run the program you must first clone the repository using 

```
git clone https://github.com/Tpanda03/ProgrammingAssignment330.git
```

then to run the program use python3 on a linux enviroment, like Ubuntu
if you do not have python, make sure to install it

```
python3 Part_1.py
```
```
python3 Part_2.py
```

## Unit test coverage:
```Python
def LockCheck(key, LockStatus):
    ...
    ...
        return LockStatus
```
This lockCheck function takes in a key, which is a numerical unlock or lock value and the current LockStatus which tells us if the access is currently locked and unlocked. This code block, or method, is called when the correct sequence is entered to the keypad.

```Python
def getDigit(number, n):
    return number[n]
```
This getDigit function is to get the correct value needed to enter into the keypad, this is taken into account the state of the FSM, depicted by n, and our code, depicted by number. 

## The platform it's been tested on:
This has been tested on a linux enviroment, as of yet there are no known bugs.
However,
the code will raise an exception and reset state when a two or more digit number, or a non numerical value is entered.

#Author: Tejash Panda

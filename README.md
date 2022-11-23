# ProgrammingAssignment330

## Describes what the program does:
Think of simulating a security installation very similar to those installed in many offices and homes. The installation has a keypad and an engine (a controller) used to decide whether the user has entered the correct access code or not.

The keypad has ten keys, labeled from '0' to '9'. The security engine will unlock the lock when it finds the correct un-locking access code in the input string. Likewise, the security engine will lock the lock when it finds the correct locking access code in the input string.

DDDDD1 is the unlocking code
DDDDD4 is the locking code, where DDDDD are the lest significant five digits in your student ID. A204(59823)
As soon as the last digit of the access code is entered, your program will signal the action taken (lock or unlock).

## How to build and run the executable:
To run the program you must first clone the repository using 

```
git clone https://github.com/Tpanda03/ProgrammingAssignment330.git
cd ProgrammingAssignment330
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
     if key == 1 and LockStatus is True: #if unlock value is entered and lock is locked
        print("Unlocked")
        return False

    elif key == 4 and LockStatus is False: #if lock value is entered and lock is unlocked
        print("Locked")
        return True

    else:
        if (key == 1) or (key == 4): #to ensure security
            if LockStatus is True:
                print("... Still Locked")
            else:
                print("... Still Unlocked")
        else:
            print("...")
        return LockStatus
```
This lockCheck function takes in a key, which is a numerical unlock or lock value and the current LockStatus which tells us if the access is currently locked and unlocked. This code block, or method, is called when the correct sequence is entered to the keypad.

```Python
def getDigit(number, n):
    return number[n]
```
This getDigit function is to get the correct value needed to enter into the keypad, this is taken into account the state of the FSM, depicted by n, and our code, depicted by number. 

in Part 2
```Python
def DoorCheck(door):
    if door is False:
        print("Unlocked")
    else:
        print("Locked")
    return door
```
in Part 2 we are to check the door after every attempt, this is the function to see if the door is unlocked or locked after our most recent attempt

## The platform it's been tested on:
This has been tested on a linux enviroment, as of yet there are no known bugs.
However,
the code will raise an exception and reset state when an incorrect or a non numerical value is entered.

#Author: Tejash Panda

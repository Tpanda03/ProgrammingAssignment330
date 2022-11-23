# ProgrammingAssignment330

## Describes what the program does:
Think of simulating a security installation very similar to those installed in many offices and homes. The installation has a keypad and an engine (a controller) used to decide whether the user has entered the correct access code or not.

The keypad has ten keys, labeled from '0' to '9'. The security engine will unlock the lock when it finds the correct un-locking access code in the input string. Likewise, the security engine will lock the lock when it finds the correct locking access code in the input string.

For example, let's assume that the un-locking code is 33441. If the user enters the string 91352033441245, then the lock will be unlocked as soon as the engine finds the last correct letter of the access code in the input string. The engine will lock the lock again when the user enters the locking code. Assuming that the locking code is 33444 then the lock will be locked and unlocked as described below:

913520334412451033444123970001112334451334410101
  unlock--^         ^--lock        unlock--^
Your program will read from standard input without echoing the input characters. Characters other than digits 0 throuh 9 will be quietly discarded. Your engine will recognize a fixed access code. The access code will be the least significant five digits in your student ID, followed by a 1 for the unlock code and by a 4 for the locking code.

DDDDD1 is the unlocking code
DDDDD4 is the locking code, where DDDDD are the lest significant five digits in your student ID.
As soon as the last digit of the access code is entered, your program will signal the action taken (lock or unlock).

## How to build and run the executable:
###

## How to generate unit test coverage:
###

## The platform it's been tested on:
###

#Author: Tejash Panda

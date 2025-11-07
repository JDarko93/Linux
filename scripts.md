# Create reusable scripts using Bash

### Bash scripts
Reusable sets of bash terminal commands can be created using the bash script. Bash scripts can run any command that can be run in a terminal
### Bash Shebang
Bash script files start withh '#!bin/bash'. This special line tells the computer to use bash as the interpreter


### Bash script arguments
Arguments can be added to a bash script after scripts name. Once provided they can be accessed by using $(position in the argument list) First argument $1, second argument $2 etc

```
#!/bin/bash
# For a script invoked by saycolors red green blue
# echoes red
echo $1

# echoes green
echo $2

# echoes blue
echo $3

```

### Bash script variables
Variables in a bash script are set using = and accessed using $
```
greeting="Hello World!"

echo $greeting
```

### read Keyword
#!bin/bash
The 'read' command can be used to prompt a user for input. It will continue to read user input until the Enter key is pressed.

Some promt text can also be specified using '-p' with the 'read' command
'''
echo "Press Enter to continue"
read
read -p "Enter your name: " name
'''


### Bash Aliases
Aliases can be created using the keyword 'alias'. They care used to create shorter commands for calling bash scripts. They can also ve used to call bash scripts with certain arguments
'''
# For example, to create an alias that invokes the saycolour script
# Script with the argument "green", the following syntax is used

alias saygreen='./saygreen.sh "green"
'''


### Bash script comparison operators 
In bash scripting, strings are compared using == (Equal) and != (Not equal) operators 

'''
#Example
#!bin/bash

word1="Hello"
word2="Hello"
word3="Hello"

if [ $word1 == $word2 ]
then
  echo "Strings are equal"
fi

if [ $word1 != $word3 ]
then
  echo "Strongs are not equal"
fi
'''
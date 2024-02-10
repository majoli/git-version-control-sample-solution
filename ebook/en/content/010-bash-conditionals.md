# Bash Conditionals

In the last section, we covered some of the most popular conditional expressions. We can now use them with standard conditional statements like `if`, `if-else` and `switch case` statements.

## If statement

The format of an `if` statement in Bash is as follows:

```bash
if [[ some_test ]]
then
    <commands>
fi
```

Here is a quick example which would ask you to enter your name in case that you've left it empty:

```bash
#!/bin/bash

# Bash if statement example

read -p "What is your name? " name

if [[ -z ${name} ]]
then
    echo "Please enter your name!"
fi
```

## If Else statement

With an `if-else` statement, you can specify an action in case that the condition in the `if` statement does not match. We can combine this with the conditional expressions from the previous section as follows:

```bash
#!/bin/bash

# Bash if statement example

read -p "What is your name? " name

if [[ -z ${name} ]]
then
    echo "Please enter your name!"
else
    echo "Hi there ${name}"
fi
```

You can use the above if statement with all of the conditional expressions from the previous chapters:

```bash
#!/bin/bash

admin="devdojo"

read -p "Enter your username? " username

# Check if the username provided is the admin

if [[ "${username}" == "${admin}" ]] ; then
    echo "You are the admin user!"
else
    echo "You are NOT the admin user!"
fi
```

Here is another example of an `if` statement which would check your current `User ID` and would not allow you to run the script as the `root` user:

```bash
#!/bin/bash

if (( $EUID == 0 )); then
    echo "Please do not run as root"
    exit
fi
```
# Bash Arguments

You can pass arguments to your shell script when you execute it. To pass an argument, you just need to write it right after the name of your script. For example:

```bash
./devdojo.com your_argument
```

In the script, we can then use `$ 1` in order to reference the first argument that we specified. 

If we pass a second argument, it would be available as `$ 2` and so on.

Let's create a short script called `arguments.sh` as an example:

```bash
#!/bin/bash

echo "Argument one is $1"
echo "Argument two is $2"
echo "Argument three is $3"
```

Save the file and make it executable:

```bash
chmod +x arguments.sh
```
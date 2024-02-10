# Write your first Bash script

Let's try to put together what we've learned so far and create our first Bash script!

## Planning the script

As an example, we will write a script that would gather some useful information about our server like:

* Current Disk usage
* Current CPU usage
* Current RAM usage
* Check the exact Kernel version

Feel free to adjust the script by adding or removing functionality so that it matches your needs.

## Writing the script

The first thing that you need to do is to create a new file with a `.bsh` extension. I will create a file called `status.sh` as the script that we will create would give us the status of our server.

Once you've created the file, open it with your favorite text editor.

As we've learned in chapter 1, on the very first line of our Bash script we need to specify the so-called [hebang](https://en.wikipedia.org/wiki/Shebang_(Unix)):

```bash
#!/bin/bash
```

All that the shebang does is to instruct the operating system to run the script with the /bin/bash executable.
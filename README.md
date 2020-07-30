# Variables vs Environment variables
Variables are system variables - they stores a value

enviroment vairalbels are related to the enviroment you have created 
enviroment variables only stay within the enviroment 

- How to create a variable in Linus
```
name= "engi67"
```
- How to display variable value
```
echo $name
```
- Store command value in your var and display

```
 dir=$(pwd)
```
- use dir to display current location

- How can we check the current env variable available in the system

This command shows what's available inside the machine:

```
env
```

- To add to the env variables within vm, you use a command called export name, for example:

```
export name ="eng-67"
```


- Adding a command's result to a variable, for example:

```
dir=$(pwd)
echo $dir
```

This will print out the current path of the directory.


- To add to the environment, you have to use the export function:

```
export DB_HOST="mongodb://192.168.10.111:27017/posts"
```

This will add to the current environment of the VM. However, if we wanted to close the VM, the env 
would not have the same variable. To prevent this, and keep it consistent, we edit the .profile file
in the root of the VM and add it there. To make sure that any profile that is created follows the
same function, we also add into .bashrc, which is one of the main root files determining the VM's 
execution.

Once we log back into the VM, it should be still there in the environment of the VM after the closure.

To test and check the environment of the VM:

```
env
```



# Shell

Shell is CLI(Command line interface) that interprets/executes/validates the commands. 

# Shell script

* A file containing sequence of shell commands.
* It can include variables, functions, loops, conditions, etc.
* Interpreted, executed by shell.

There are different types of shells like Zshell, CShell, Kshell. But Bash is popular and recent that includes all the features.

**NOTE: Consider Bash shell or Shell both are same**

# How to call another shell script from current shell script
* If you need to preserve variables and functions from the current shell in the second script, use source or ..
* If you want to run the second script in a separate shell process, use sh or bash.
* If you want to replace the current shell with the second script, use exec.
* If you want to execute the contents of the second script as if they were typed directly into the current shell, use eval.
* If you want to define a function to call the second script, use function.

```bash

#!/bin/bash

# Current script
echo "This is the current script."

# Call the second script using source
source second_script.sh

# Call the second script using sh
sh second_script.sh
```

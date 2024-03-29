## Custom Shell Command Creator

### Usage

- If you are using windows, download [Git](https://git-scm.com/download/win), which will install Git Bash as well. Then open Git Bash and run following commands

### Step 1.
In the shell run:
- `$ git clone https://github.com/braindotai/Custom-Shell-Command-Creator.git`
- `$ cd Custom-Shell-Command-creator`
- `$ chmod +x commander`
- `$ mkdir ~/bin`
- `$ cp commander ~/bin"`
- `$ echo 'export PATH=$PATH":$HOME/bin"' >> .profile`

Then go back to working directory
- `$ cd ..`


### Step 2.
Create any python file that you want to convert into a shell command, and save it.
For example-
```python
import sys
for arg in sys.argv[1:]:
    print(arg)
```
Save it as commandname.py


Then run `$ commander <name of the python file without extention>`

That is, `$ commander commandname`

Make sure that you are running "commander" where the that python file is saved.

### Step 3.
Now you can simply run the command by the name of your python file

For example:

```
$ commandname arg1 arg2
arg1
arg2
```

You can delete the cloned repository if you want to.

# __ENJOY__
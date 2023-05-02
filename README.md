# todos
Python script to find and print TODOs in given route (current dir by default)  

## Caution
Make sure to not run todos in a large parent directory, like your home folder. There are probably lots of `.py` files you are not aware of, so the script will find all of them and print lots of TODOs. Press Ctrl+C if this happens.

## Why
Just write TODO:s over your project code. This script will print them out for you in case you want a reminder for all of them. Nice way to keep track of TODOs for solo projects or small teams. The script ignores specific files and dirs, you can edit that at the top.

## How to use
1. Move the script to your `/usr/local/bin/`
```fish
sudo mv todos /usr/local/bin
```  

2. Give executable permissions.  

```fish
sudo chmod +x /usr/local/bin/todos
```  


3. Now you can run todos anywhere.

```fish
cd my/project/
todos
```  

```
TODOS
my/project/main.py:26       # Fix this bug here
my/project/module/core.py:1 # Add comments
```

4. You can also give the absolute path to todos and it will work.
```fish
cd Desktop
todos /path/to/my/project
```  
   
## TODO:
Prioritys could be added so TODOs can be ranked before they are printed.  

`# TODO:Priority Level: Fix this bug here`

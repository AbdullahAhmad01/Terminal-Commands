# Terminal-Commands
Some Useful Linux Terminal programs

## 1  flmod
  The program is used for two main purposes:
    1. Creating files of given mode
    2. Creating script files

#### Examples
**1:**
```bash
flmod 644 details.txt
```
equivilant to `touch details.txt ; chmod 644 details.txt`

**2:**
```bash
flmod -o 644 details.txt
```
same as first example but delete file if exists

**3:**
```bash
flmod -s myscript
```
Create 'myscript' file in current working directory, write following content in 'myscript' and finally run it
```bash
#!/bin/bash

# myscript : describe your program in one line

echo "Script file is ready"
```

**4:** 
```bash
flmod -s -e myscript
```
same as 3 but also open script using `nano myscript`

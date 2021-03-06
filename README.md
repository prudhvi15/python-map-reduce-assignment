# Python Map Reduce

Basic Python introduction and concepts needed in preparation for working with map-reduce solutions.

## Requirements

- Install Chocolatey, the Windows package manager
- Install the Anaconda 3 version for Python + common packages
- Install Visual Studio Code for text editing
- Add Open Command Window Here as Administrator to your File Explorer context menu.

```PowerShell
- choco install anaconda3 -y
- choco install vscode -y
```

## Case 1:  Local file-based

```
python 11mapper.py
python 12sorter.py
python 13reducer.py
```

## Case 2:  Use standard input and output

Use the console (standard input and output) and shell commands to pipe information.  We'll use the built-in shell sort command, so we don't need that anymore. 

cat data | map | sort | reduce

PowerShell and Bash use the same commands:

```Bash
cat part.txt
cat part.txt | python 21mapper.py
cat part.txt | python 21mapper.py | sort
cat part.txt | python 21mapper.py | sort  | python 22reducer.py

```
Commands to process larger data file:

```
cat purchases.txt
cat purchases.txt | python 21mapper.py
cat purchases.txt | python 21mapper.py | sort
cat purchases.txt | python 21mapper.py | sort  | python 22reducer.py
```

## References

- [Udacity "Introduction to Hadoop and MapReduce"](https://classroom.udacity.com/courses/ud617/)
- [IBM Python for Data Science](https://cognitiveclass.ai/courses/python-for-data-science)
- [Basic Setup for Big Data](https://github.com/denisecase/basic-setup-for-bigdata)

## Repository
- Forked from [https://github.com/denisecase/python-map-reduce](https://github.com/denisecase/python-map-reduce)
- My repo [https://github.com/prudhvi15/python-map-reduce-assignment](https://github.com/prudhvi15/python-map-reduce-assignment)

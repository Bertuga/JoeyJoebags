# JoeyJoebags
Custom version of the Joeybags software.


## Current Additions
- Fixes dumping 32MB repros like the DV15 & PPP08
- Allow dumping of 2048M Roms for dumping 369 In 1 carts
- Dumping / Flashing completion percentage
- Progress is now shown on a single line


# Compiling/Decompiling Windows Binaries

### Compiling
Run ```python -m py2exe JoeyJoebags***.py``` and windows binaries will be compiled.

### Requirements
```
Python 3.4
PyUSB
py2exe
```

### Installing Requirements
1. Download & Install Python 3.4 64bit from https://www.python.org/downloads/windows/
2. open cmd as admin and type ```python -m pip install PyUSB``` & ```python -m pip install py2exe```

### Decompiling
To decompile the binary you will need python_exe_unpack.py from https://github.com/countercept/python-exe-unpacker just follow the instructions in the readme, to decompile the exe use ```python python_exe_unpack.py -i JoeyJoebags.exe```

If you experience any issues with installing PyCrypto for the decompiler, install this https://github.com/axper/python3-pycrypto-windows-installer

### Requirements
```
Python 3.4
pefile
unpy2exe
uncompyle6
xdis
pycrypto
configparser
```

### Installing Requirements
1. Download & Install Python 3.4 64bit from https://www.python.org/downloads/windows/
2. Download https://github.com/countercept/python-exe-unpacker
3. open cmd as admin in the python-exe-unpacker folder and type ```python -m pip install -r requirements.txt```
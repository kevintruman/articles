# Install Python Embeddable Package (Binary) V3

### Download And Install Python Embeddable Package

Download the software

- windows: https://www.python.org/downloads/windows/

- linux: https://www.python.org/downloads/source/

- macos: https://www.python.org/downloads/macos/

Extract to your program directory (without run administrator or root), 
example: `C:\src\prog\python`

Add environment variable `C:\src\prog\python` and `C:\src\prog\python\Script`

example for windows: 
```
> set PYTHON_HOME=C:\src\prog\python
> set PYTHON_SCRIPT=C:\src\prog\python\Script
```

example for linux:
```
$ export PYTHON_HOME=/data/prog/python
$ export PYTHON_SCRIPT=/data/prog/python/Script
```
 
Check python already installed
```
$ python --version
```


### Install `pip`

Open directory python installed, edit file `python3xx._pth` and uncomment `import site`

```
python311.zip
.

# Uncomment to run site.main() automatically
import site
```

Download `get-pip.py` script for install pip binary on https://bootstrap.pypa.io/get-pip.py

Input command below for installation pip
```
$ python get-pip.py
```

Check pip already installed
```
$ pip --version
```
or
```
$ python -m pip --version
```

### Install `virtualenv` (`venv`)

Input command
```
$ python -m pip install virtualenv
```

check virtualenv already installed
```
$ virtualenv --version
```
or
```
$ python -m pip --version
```

### Note

- `-m` command for call module in library python


### Articles Source

- https://pip.pypa.io/en/stable/installation/
- https://stackoverflow.com/questions/42666121/pip-with-embedded-python
- https://stackoverflow.com/questions/33181071/why-is-python-saying-i-have-no-module-named-venv
- https://docs.python.org/3/library/venv.html


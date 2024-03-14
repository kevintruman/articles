# Use `virtualenv` (`venv`) Python Project

### Install

If you install executable python, skip this step. 
Because in executable installation already installed `venv`. Or check
```
$ python -m pip venv --version

or

$ python -m pip virtualenv --version
```

Start installation
```
$ python -m pip install virtualenv 
```

### Create Project

Create directory project, example:
```
$ mkdir firstenv
$ cd firstenv
```

Create virtualenv directory
```
$ python -m pip virtualenv <dir_env_name>

or 

$ python -m pip venv <dir_env_name>
```

example:
```
$ python -m pip virtualenv venv
```

Then directory `venv` created

### Active `virtualenv`

```
$ ./venv/Scripts/activate
```

### Deactivate `virtualenv` (Windows)

```
> venv\Scripts\deactivate.bat
```

### Export Library Project (`requirements.txt`)

Two ways to export library, use `pip freeze` and `pipreqs`.
`pip freeze` will get all the library installed, `pipreqs` will generate only library using in project. 

Using `pip freeze`
```
$ pip freeze > requirements.txt
```
will generate `requirements.txt` file in current/project directory

Using `pipreqs`, install first
```
$ pip install pipreqs
```

Export library
```
$ pipreqs
```
generate `requirements.txt` file in current/project directory, or custom directory
```
$ pipreqs <dir_export> --force

example:

$ pipreqs ./libs --force
```

Note: `--force` for replace `requirements.txt` file existing

### Import Library Project From `requirements.txt` File

```
$ pip install -r requirements.txt
```

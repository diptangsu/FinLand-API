# FinLand-API
API for FinLand android app made using Flask. HackerEarth BTS Hackathon


# Setup
Make sure you have `python3.6` installed in your machine before you continue. For windows users, the path to `python3.6` must be added to the system environment variable `PATH`.  
Install virtualenv in python. `pip3 install virtualenv`

## Create a virtual environment
### Linux
```bash
$ virtualenv -p python3 venv
```
This will create a virtual environment named venv with python3 as its interpreter.

## Windows
If you have multiple versions of python installed and added to `PATH` follow the following steps.  
```cmd
> where python
C:\Python27\python.exe
C:\Users\deepd\AppData\Local\Programs\Python\Python37-32\python.exe
C:\Users\deepd\AppData\Local\Programs\Python\Python36\python.exe
```
You will get an output of all the python execuables that are added to `PATH`. For example I have `python2.7`, `python3.6` and `python3.7` installed.

Use the path of `python3.6` to create the virtual environment.
```cmd
> virtualenv -p C:\Users\deepd\AppData\Local\Programs\Python\Python36\python.exe venv
```

## Activating the virtualenv
### Linux
```bash
$ source venv/bin/activate
(venv) ...$ 
```
### Windows
```cmd
> venv\Scripts\activate
(venv) ...> 
```

## Installing requirements
You can either install requirements from the [requirements.txt](/requirements.txt) file but using the command  
```
pip install -r requirements.txt
```
or manuallly using
```
pip install Flask Pillow tensorflow keras
```

## Running the API
Run the [api.py](/api.py) file to start the API server.  
`python api.py`
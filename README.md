# LearningFastAPI 

## Introduction
FastAPI is a quick learn backend developing language, and its very easy to learn as it is mainly python based. The main operations that are used to perform backend tasks are known as post and fetch.
The handling of data is basically in the form of a JSON object, which looks like this

 ```json
{ 
    "name": "Farhan",
    "age": 21,
    "skills": ["Python", "Java", "Quantum Computing"] 
}
 ```

 ## Setting-up the environment
 So before, that lets create an environment in the VSCode so that global variables do not interfere with the variables and modules that will be installed in your directory, so to install a virtual environment we install the venv module, whose documentation you can also check on the [venv documentation](https://docs.python.org/3/library/venv.html).

 ### Step 0: Download this repository to your local computer
 If you dont download how are you gonna access some files from my repository???


### Step 1: Install the virtual environment

 To install a virtual environment we create a folder in which we want to install and open the folder in terminal and write the following 


 ```bash
python -m venv <environment_name>
```


for this project I am taking the environment name to be as "fast-api"


### Step 2: Create the virtual environment

For Windows


```bash
.\<environment_name>\Scripts\Activate.ps1
```


For Linux/Mac:


```bash
source <environment_name>/bin/activate
```

You shall even notice this change in your terminal
From 


```bash
PS C:\User\...>
```


TO 


```bash
(<environment_name>) PS C:\User\...>
```


### Step 3: Install the necessary modules

Now we install the most necessary module, that is fastapi


```bash
pip install fastapi uvicorn
```


But for your ease I have provided a requirements.txt file add it to your folder and then just run this command on terminal


```bash
pip install -r requirements.txt
```


This command installs all the modules mentioned in the requirements.txt file.
Now you are all good to go.

## Your first FastAPI app 
Now FastAPI depends on two main functions, post and get these is the backbone of the backend. Now to make your first api, create a file named "main.py", I am writing the code for you, but after this you are gonna do it yourself


```python
from fastapi import FastAPI

app = FastAPI()

@app.get("/")
def homepage():
    return {"message": "HI"}

```


To run the server we write the following command on the terminal


```bash
uvicorn main:app --reload
```


We use --reload so that it automatically relaods the server as soon a change is saved in 
main.py . But its not always necessary to follow all the pneumatics for example 


```text
uvicorn main:app --reload
        ^     ^
  python file |
              |
        FastAPI app name
```

Now after running the above command. You must get an output similar to this

```bash
INFO:     Will watch for changes in these directories: ['C:\\User\\...']
INFO:     Uvicorn running on http://127.0.0.1:8000 (Press CTRL+C to quit)
INFO:     Started reloader process [2280] using StatReload
INFO:     Started server process [10748]
INFO:     Waiting for application startup.
INFO:     Application startup complete.
```
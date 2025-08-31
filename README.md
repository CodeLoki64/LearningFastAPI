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



### Step 3: Install the necessary modules

Now we install the most necessary module, that is fastapi


```bash
pip install fastapi uvicorn
```

But for your ease I have provided a requirements.txt file and then just run this 
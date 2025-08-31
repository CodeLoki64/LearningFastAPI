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

 To install a virtual environment we create a folder in which we want to install and open the folder in terminal and write the following 


 ```bash
python -m venv <folder_name>
```


for this project I am taking the folder name to be as "fast-api"
Now we install the most necessary module, that is fastapi


```bash
cd install fastapi uvicorn
```


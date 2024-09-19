# Creating Virtual Environments

Terminal in VS code can be used to code in linux way using Powershell or Git Bash.

Good practice to create environments to seggregate the packages from further updates which are coming on the packages. But here we will be going ahead with command terminal which is specific to windows.

As we have already installed conda, so we will use conda to create the environment. The course will be done using Python ver 3.10.

To create a virtual environment `venv` use the following code:

```
conda create -p venv python==3.10
```

`-p venv`: The `-p` flag indicates that you want to specify a path, and `venv` is the directory path where the environment will be created. If `venv` is a relative path, it will be created relative to your current working directory.

After running the above code, activate the environment using __conda activate venv/__: (Don't ignore the slash at the end.)
```
D:\Github\Udemy-ML_NLP_course>conda activate venv/
(D:\Github\Udemy-ML_NLP_course\venv) D:\Github\Udemy-ML_NLP_course>                
```

Now to add the packages names here make sure that the names are crrectly written in the __requirements.txt__. And write the code:

```
pip install -r requirements.txt
```

To clean the command terminal screen use the command:
```
cls
```
Below image, observe how the the `test.py` file was run. The `venv` has all the libraries needed for it. 

![](images\1.PNG)

To run jupyter notebook in VS code we need some packages - __ipykernel__ (its responsible for providing a specific kernel to jupyter notebook file.)

Once you open a jupyter notebook, select kernel and use the created __venv__.
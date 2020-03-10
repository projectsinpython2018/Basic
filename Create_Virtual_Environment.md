# Virtual Environment 


In this document, I will explain some basic parts for to be expert and have different python versions on your OS. 
Note: As you know, the python version 2.7 will be expired until 2020. 

So let's do it, although it is explained in different websites, I just mentioned some basic parts to use it. 

1. First of all Install the virtualenv packages on your main python : 

    `$ pip install virtualenv`
  
2. Check the version of the virtaulenv package: 
  
    `$ virtualenv --version`
   
3. Create your own virtual enviroment : (my_name : is optional)
  
    `$ virtualenv my_name`
  
    Note: After doing it code your enviroment is created on the current location so you need to learn working on `git` and `terminal` for changing the directory and making something important on your code. 
  
4. Python versions : 
    
    Python 3:
    `$ virtualenv -p /usr/bin/python virtualenv_name`
    
    Python 2.7: 
    `$ virtualenv -p /usr/bin/python2.7 virtualenv_name`
    
5. Until now, you just create it, but you can activate it using this:

    `$ source virtualenv_name/bin/activate`
  
6. When you run this virtual and activated, it shows like this and from now on you can have your own packages with specific version that you want. 
  
    `(my_name)$ pip install Numpy==1.9`
  
7. After runnig your code, you just need to deactivate your virtaulenv :
 
    `(my_name)$ deactivate`


Until now you have learnt how to create your own VirtaulEnv on your os, but now we need work on Jupyter Notebook: 

1. when you are in current location on your terminal :

    `$ ipython kernel install --user --name my_name`
  
More and Advance Options : 

1. If you working on github as team or you want to run your project on other OS you should have some packages version: 

    Note : Requirements is defult name but you can change it. 
    
    `$ pip freeze > <location/requirements.txt>`
  
2. For installing your packages on different OS you just need to script it: 
  
    `$ pip install -r <source/requirements.txt>`

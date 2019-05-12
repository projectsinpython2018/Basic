# Virtual Environment 


In this document, I will expalin some basic parts for being expert and have different pythons version on your OS. 
Note: As you know, the python version 2.7 will be expired until 2020. 

So let's do it, although you can see different websites that expalin it but i just mention some basic parts and you can use it. 

1. First of all Installing the virtualenv packages on your main python : 

    `$ pip install virtualenv`
  
2. Check the version of the virtaulenv package: 
  
    `$ virtualenv --version`
   
3. Create your own virtual : (my_name : is optional)
  
    `$ virtualenv my_name`
  
    Note: After doing this code your enviroment is created on the current location so you should learn work on `git` and `terminal` for change the directory and make something important on your code. 
  
4. Python versions : 
    
    Python 3:
    `$ virtualenv -p /usr/bin/python3 virtualenv_name`
    
    Python 2.7: 
    `$ virtualenv -p /usr/bin/python2.7 virtualenv_name`
    
5. Until now, you just create it, but how you can use it?

    `$ source virtualenv_name/bin/activate`
  
6. When you run this virtual and activated, it shows like this and from now on you can have your own packages with specific version that you want. 
  
    `(my_name)$ pip install Numpy==1.9`
  
7. Finish, When you run your code and finish it, you just need to deactivate your virtaulenv :
 
    `(my_name)$ deactivate`


Until this part you learn how to create your own VirtaulEnv on your os, but now we need work on Jupyter Notebook: 

1. when you are in current location on your terminal :

    `$ ipython kernel install --user --name = my_name`
  
More and Advance Options : 

1. If you working on github as team or you want to run your project on other OS you should have some packages version: 

    Note : Requirements can change but defualt name is Requerments. 
    
    `$ pip freeze > <location/requirements.txt>`
  
2. For install your packages on different OS you just need run this code on current location: 
  
    `$ pip install -r <source/requirements.txt>`

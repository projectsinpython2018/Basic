# Conda Virtual 

In [previous post ](https://github.com/projectsinpython2018/Basic/blob/master/Create_Virtual_Environment.md#virtual-environment)explain about `Virtualenv`, and why we need that.
This document explain how to create a `conda virtualenv` for whose use Anaconda. 
Anacoda creates easy pathway for virtualenv, it's such straight forward. Lets look at it: 
## Note: Because it's about coding on python, I use `#` for comment. 

`# Change Directory (cd) to [file]`

`> cd [file]`

`# Time to create conda virtualenv` 

`> conda create -n [name_of_virtualenv] python=3.x #[x:python version like 3.6]`

`> conda activate [name_of_virtualenv]`

We need another something more to have accurate python virtualenv. That's requiremtns packages. In this part of our configuration we use TechnologyScout.net, you can read more in [this](https://www.technologyscout.net).

`> while read requitments;do conda install --yes $requirments; done < requirments.txt`

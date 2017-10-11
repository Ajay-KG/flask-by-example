### Refernce : 
    https://realpython.com/blog/python/flask-by-example-part-1-project-setup/
    https://stackoverflow.com/questions/44521712/heroku-commands-and-push-giving-me-cli-is-deprecated-please-reinstall-error

### Project Setup

    Linux (Ubuntu etc)
        ##### Intsall prerequisites of development environment libraries
      
            sudo apt-get update
        
            sudo apt-get install python-setuptools python-dev build-essential git-core -y
        
            sudo easy_install pip
          
        ##### Use virtual env, It is optional but better to use to avoid dependency conflicts
    
            sudo pip install virtualenv
        
            sudo pip install virtualenvwrapper
        
            mkdir ~/virtualenvs 
        
            echo "export WORKON_HOME=~/virtualenvs" >> ~/.bashrc
        
            echo "source /usr/local/bin/virtualenvwrapper.sh" >> ~/.bashrc 
        
            echo "export PIP_VIRTUALENV_BASE=~/virtualenvs" >> ~/.bashrc 
        
            source ~/.bashrc 
    


    For Mac
    
        Install pip => http://pip.readthedocs.io/en/stable/installing/
    
        ##### virtual environment set
    
            pip install virtualenv
            virtualenv --version
        
            pip install virtualenvwrapper
            which virtualenvwrapper.sh
        
            mkdir ~/Workspace/virtualenvs
            which virtualenvwrapper.sh
            echo "export WORKON_HOME=~/Workspace/virtualenvs" >> ~/.bash_profile
        
            echo "export WORKON_HOME=~/Workspace/virtualenvs" >> ~/.bash_profile
            echo "source /usr/local/bin/virtualenvwrapper.sh" >> ~/.bash_profile
        
            echo "export PIP_VIRTUALENV_BASE=~/Workspace/virtualenvs" >> ~/.bash_profile
        
            source ~/.bash_profile


##### Virtual env wrapper commands

	1. **mkvirtualenv:** To create a new environment. Example: mkvirtualenv blog
	2. **deactivate:** To get out/off your virtualenv. Example: deactivate
	3. **workon:** To jump back on the virtualenv. Example: workon blog
	4. **rmvirtualenv:** To remove the virtualenv. Example: rmvirtualenv blog


##### Install project requirements

```
pip install -r requirements.txt
```


```
follow this to run flask project on PyCharm https://github.com/pallets/flask/blob/master/docs/cli.rst
```

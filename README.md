# ml-training


Launching Jupyter with your desired version of python

## prerequisites
* pyenv
* pipenv
* add 
```
    # make python use the global pyenv python version
    eval "$(pyenv init --path)"
    # make pipenv use the system python ( pyenv )
    alias pipenv='pipenv --python=$(which python)'
```
to your ~/.bash_profile

* run `pipenv shell` - this creates a virtualenv and runs a shell in it. Not sure why, but running this deletes the old environment and creates a new one every time.
* run `pipenv install` - this installs all the dependencies from the Pipfile
* run `pipenv run jupyter notebook` - this will launch jupyter on localhost
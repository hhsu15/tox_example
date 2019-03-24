# tox tutorial

- create file called `tox.ini`

- show tox information, tells you the default env
```
tox -av
```
- show evrything config you can do!!
```
tox --showconfig

```
- add verbosity, showing you what tox is really  doing!
```
tox -vvvvv

```

- run test environment
```
tox -e dev2  # run only test environment dev2

```

# create development environment
- make sure you have setup.py file(that has packages = find_packages())
- use pip install --edidable to install your project
- this is installed in the development mode (but only for dev, not really living in the site-pacage folder
```
pip install -e . # pass the project as the args
pip list  # then you will see your project in your packages
```
- In tox, to do the same thing(creating dev mode), simply use
```
usedevelop = True # same as pip install -e .
```


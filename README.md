# I513-Project

# How do I install the project dependencies?

```
$ pip3 install -r requirements.txt
```

# How do I add a package to our dependencies?

Find your package. Lets assume sklearn:

```
$ pip3 freeze | grep sklearn
sklearn==0.0
```

```
$ echo "sklearn==0.0" >> requirements.txt
```


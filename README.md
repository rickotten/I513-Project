# I513-Project

# What is the Pipfile?

It is a file that manages the pip dependencies for our project. For example, pandas and sklearn are in there.

# Why do we need a Pipfile?

It is always wise to use virtual environments whenever possible. For example, if you install a faulty package that
breaks pip, then naturally you don't want it to break your root pip. Otherwise you'll have a potential nightmare on
your hands.

This also makes dependencies easy to manage accross our group. If one were to add `numpy` as a dependency, then the others
would not know about it until they ran into an error: "missing numpy". So this allows us to easily keep track and install
all things at once.

The Pipfile corresponds to a pipenv (which is a variant of python venvs. Very easy to use)

# How to I use the Pipfile?

Well first you need to install pipenv into your root pip. Something like the following:

```
$ pip install pipenv
```

# How do I install all our current dependencies?

Easy. `pipenv install` from the root directory of the repo. (ie. the directory where the Pipfile exists!)

# How do I add a new package to our dependencies?

Easy again. For example, `pipenv install numpy`. You will notice that Pipfile itself changes as you install new things.
Since it's a file tracked by git, we have a way of tracking our dependencies.

# How can I enter this virtual environment?

Easy. From the root directory of the repo (where the Pipfile exists), run `pipenv shell`. Done.



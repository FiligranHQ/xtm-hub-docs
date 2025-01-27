# XTM Hub Documentation Space

## Introduction

This is the main repository of the XTM Hub Documentation space. The online version is available directly on [docs.openbas.io](https://docs.openbas.io).

## Install the documentation locally

### Clone the repository
```sh
$ git clone git@github.com:OpenBAS-Platform/docs.git
```

### Prepare the environment
```sh
$ cd docs
$ python3 -m venv venv
```

#### MacOS/Linux:
```sh
$ source venv/bin/activate
```

#### Windows:
```sh
$ venv\Scripts\Activate.ps1
```

### Install dependencies
```sh
$ pip install -r requirements.txt
```

### Launch the local environment:
```sh
$ mkdocs serve
Starting server at http://localhost:8000/
```

## Deploy the documentation

### Update the source

Commiting on the main branch does not impact the deployed documentation, please commit as many times as possible:
```
$ git commit -a -m "[docs] MESSAGE"
$ git push
```

### Deploy and update the current version

With the right version number (eg. 3.3.X):
```
$ mike deploy --push [version]
```

### Deploy a new stable version

With the right version number (eg. 3.3.X), update the `latest` tag:
```
$ mike deploy --push --update-aliases [version] latest
```

## Useful commands

```sh
$ mike help
usage: mike [-h] [--version] [-q] [--debug] COMMAND ...

mike is a utility to make it easy to deploy multiple versions of your MkDocs-powered docs to a Git branch, suitable for deploying to Github via gh-pages. It's designed to produce one version of your docs at a time. That way, you can easily deploy a new version
without touching any older versions of your docs.

positional arguments:
  COMMAND
    deploy              build docs and deploy them to a branch
    delete              delete docs from a branch
    alias               alias docs on a branch
    props               get/set version properties
    retitle             change the title of a version
    list                list deployed docs on a branch
    set-default         set the default version for your docs
    serve               serve docs locally for testing
```

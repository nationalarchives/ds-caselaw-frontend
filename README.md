# Introduction
This repository is a [template repository](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template).

When you want to create a new DA repository, you should do so by using this template.  Hint: click the green button above that says "Use this template".

# Why
We want to ensure that all repositories in DA follow defined conventions and standards. See [The Engineering Handbook](https://national-archives.atlassian.net/wiki/spaces/DAAE/pages/47775767/Engineering+Handbook).

Specifically, this mandates that all repositories implement at least these minimal set of [pre-commit](https://pre-commit.com/) hooks and a pre-commit check.  Update these as you see fit - if you need to.

It is therefore required that you use [pre-commit](https://pre-commit.com/) and the [detect secrets](https://github.com/Yelp/detect-secrets) tool/hook.

They can generally be installed with pip. e.g.

```
pip install pre-commit
pip install detect-secrets
```

You will need to initialise pre-commit after cloning the newly created repository by running:

```pre-commit install```

# Contents
```README.md``` - Change this as appropriate.

```CHANGELOG.md``` - A [Keep a change log](https://keepachangelog.com/en/1.0.0/) changelog.

```LICENSE``` - A MIT License dated 2023 Crown Copyright.

```.pre-commit-config.yaml``` - Sensible defaults to get you started.  Add the hooks you need accordingly.

```.secrets.baseline``` - A baseline file for detect-secrets that assumes there should be no secrets in this repository.

```.github/workflows/pre_commit.yml``` - A workflow which runs pre-commit on a pull request to main, as a check.

# Protect Main Branch
Creating a repo from the template will not set branch protection.
See [The Engineering Handbook](https://national-archives.atlassian.net/wiki/spaces/DAAE/pages/47775767/Engineering+Handbook) for guidance.

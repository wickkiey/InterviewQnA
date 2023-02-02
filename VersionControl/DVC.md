# DVC

Data version control tracks the changes in the data and helps to reproduce the results. It is a command line tool that helps to version the data and models. It is a part of the [CML](https://cml.dev/) project.

## Installation

```bash
pip install dvc
```

## Initialize DVC

```bash
dvc init
```

## Add data to DVC

```bash
dvc add data.csv
```

## Push data to remote

```bash
dvc push
```

## Pull data from remote

```bash
dvc pull
```

## Check the status of the data

```bash

dvc status
```

## Check the changes in the data

```bash
dvc diff
```


Based on the dvc.xml file it can be linked to git version, so that it can be tracked in git.
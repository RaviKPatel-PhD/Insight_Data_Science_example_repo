# Insight_Data_Science_example_repo  

This Github repo contains an example of how to structure your repo for your Insight project. You do not have to follow this structure exactly, but it may be useful to clone this repo as a starting point for your own project. Here is an outline of the different files we recommend having in your project repo. Below we go into details of what exactly that directory/file should contain.

## Overview/Structure of your Insight projects Github repo:

[Name_of_repo](#Name_of_repo)
[README.md](#README)
[/Abbreviated_project_name](#Abbreviated_project_name)
[/develop](#develop)
[/config](#config)
[/pipelines](#pipelines)
[/tests](#tests)
[/docs](#docs)
[/data](#data)
[LICENSE](#LICENSE)
[pipfile](#pipfile)
[pipefile.lock](#pipfile)
[.gitignore](#.gitignore)
[.git](#.git)


## Name_of_repo
When you are starting out your project you likely don't know exactly where the project will take you, so don't worry too much about picking a name right now. You can always change the name of the repo later by clicking 'settings' on github within your repo. When you do get closer to finalizing your project we suggest naming your repo the same as the name of your project within you slide deck to stay consistent.

## README.md
This is arguably the most important file within your Github repo! If there is a file titled 'README.md' in the home directory of your repo, it will automatically become the landing page for the the repo. That means if you share your repo with someone they will see the README first and that may be the only file they look at before deciding if they should continue looking. [Here](https://gist.github.com/fvcproductions/1bfc2d4aecb01a834b46) is an example of how to structure your README. Remember the information at the top is the most important and the further down information is the less likely anyone is to read it. Its always better if you can embed images of gifs in your README to illustrate difficult concepts. That makes he README more enticing to actually read. Your README may contain a lot of information. If thats the case we highly recommend adding a table of contents to make it easier to navigate.  
The README is a markdown file and Github will automatically format any markdown files within the repo when displaying them. If you are unfamiliar with markdown [here](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) is a really useful guide. Markdown is not useful only for Github. You can also use markdown within the markdown cells in Jupyter notebooks and on the Insight Platform.

## Abbreviated_project_name
You can definitely call this directory something else. This is where all the scripts related to your project will go. It is highly recommended to have multiple files relate to your project rather than one big file containing everything. It is good to be mindful that large files can often take a long time to load in Github. Here are some example files you may have within this directory. Many of these files are python scripts, but it often makes sense to use jupyter notebooks, so feel free to do so.

**File name** | **Purpose**
--- | ---
__init__.py | .
Loading_data.py | If your data has to be loaded or scraped from the web that would be done with this scripts
Data_cleaning.py | Clean the data and get it ready for machine learning.
Exploratory_analysis.ipynb | Explore your data, make some pretty graphs. This is often easiest with a jupyter notebooks
Model_trainers.py | Here is where you may test several models, fit the pipeline of series of data transformations -> machine learning. You can learn more about sklearn pipelines [here](https://scikit-learn.org/stable/modules/generated/sklearn.pipeline.Pipeline.html)
Evaluators.py | Evaluate your model performance. Maybe include some experiments to test how your model does under different conditions.

Everyone's project is different and therefore its totally possible you will end up including way more or different files within this directory.

## develop
This directory is optional, but it may be useful to keep work in progress versions of the files in the [Abbreviated_project_name](#Abbreviated_project_name) directory here.

## config
You can store things here that were calculated during your project, such as optimal model hyper parameters.

## pipelines
You can store your final model here.

## tests
If someone where to clone your model what tests could they run to ensure its running properly? It is software engineering best practice to always have some tests to run to make sure everything is running properly. These test cases could be individual instances from the test dataset that you know the answer to. 

## docs

## data

## LICENSE

## pipfile and pipefile.lock

## .gitignore

## .git

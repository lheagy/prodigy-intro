# PRODIGY Intro Tutorial
Introduction to using Python for working with Network Common Data Form ([NetCDF](https://foundations.projectpythia.org/core/data-formats/netcdf-cf.html)) files.

## Getting Python on your machine

If you are just getting acquainted with Python, I highly recommend the [Transform 2022 tutorial: Getting Started with Python](https://transform.softwareunderground.org/2022-getting-started-python).

I recommend using either [miniconda](https://docs.conda.io/en/latest/miniconda.html) or [miniforge](https://github.com/conda-forge/miniforge#miniforge) to install python on your machine. These distributions are lightweight distributions of the package mananger [Conda](https://docs.conda.io/en/latest).

## Using Git and GitHub 

If you are looking for a tutorial, the [Transform 2021 tutorial: Version Control for Scientists](https://transform.softwareunderground.org/2021-version-control) is a good place to look; specifically Part 1: Git and GitHub. 

If you would like to create your own copy of this repository that you can make changes to, and push those changes to GitHub, you can first [fork](https://docs.github.com/en/get-started/quickstart/fork-a-repo) this repository. This is optional.

You will then need to clone this repository (or your fork). Open a terminal and run 

```
git clone https://github.com/lheagy/prodigy-intro.git
```

(If you are using your fork, replace `lheagy` with your GitHub username). 

## Setting up the environment 

You will then need to navigate to the `prodigy-intro` directory

```
cd prodigy-intro
```

and create the `prodigy-intro` environment. This will install the specific packages that we need for this tutorial. For more information on environments, see the [Conda Managing Environments Docs](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html). 

```
conda env create -f environment.yml
```

To activate this environment, you then need to run 

```
conda activate prodigy-intro
```

Environment files are a useful tool for communicating what packages someone needs to run your code and reproduce your results (`#ReproducibleScience!`). If you want to be very particular about specific package versions (useful when you will publish code alongside a paper), you can check out [conda lock files](https://github.com/conda-incubator/conda-lock#conda-lock)

## Jupyter

Jupyter is an interactive computing environment. It provides an interface where you can combine narrative text with code to capture and describe your workflow. If you are new to Jupyter or looking for a refersher, [Project Pythia has some nice documentation](https://foundations.projectpythia.org/foundations/getting-started-jupyter.html). 

You can launch Jupyter by running 

```
jupyter lab
```

## Xarray & NetCDF

We will use [Xarray to open up our NetCDF files](https://foundations.projectpythia.org/core/xarray/xarray-intro.html#opening-netcdf-data). See the notebooks for an example

## Open source practices

In 2022, I helped give a tutorial on [Best practices for sharing your research code](https://github.com/agu-ossi/2020-agu-oss). The slides, notebooks and a recording of the tutorial are available. 

In terms of some brief points to consider... 

**Data**: in general, you don't want to put large data files in GitHub. Instead, if they are public data, provide instructions for how to download those data. If you have data (or data-derived products) that you would like to share, you can use platforms such as [Zenodo](https://zenodo.org/) or [FigShare](https://figshare.com/) to archive your data with a doi. 

**License**: A repository without a license is not open-source, in fact, it is copyright of the author, meaning that no one else has permission to use it. To communicate if, and how, others can use your code, you can select a license. A good resource for helping select a license is [choosealicense.com](https://choosealicense.com/). Further, the [Open Source Initiative](https://opensource.org/) maintains a [definition of open-source](https://opensource.org/osd) and a [catalog of licenses that satisfy that definition](https://opensource.org/licenses). 

## Some great resources

- [Project Pythia: Foundations Book](https://foundations.projectpythia.org/landing-page.html)
- [Transform conference tutorials](https://transform.softwareunderground.org/overview)
- [Ocean HackWeek 2022 tutorials](https://oceanhackweek.github.io/ohw22/tutorials-index/index.html)
- [Software Carpentry Lessons](https://software-carpentry.org/lessons/)

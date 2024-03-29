# Conda, Python and R

## Python and R learning resources

While we anticipate that most participants will have some experience with Python and/or R programming, we understand that everyone joining OceanHackWeek is coming from a different background and skill level in programming. Below are links to a few resources to refresh your skills in Python and R, as well as a tutorial video from a previous OHW event that covers a handful of Python packages. The material covered in these lessons is a good reflection of the level we expect participants to be at and should get you up-to-date on the basic programming skills needed for the workshop.

- [Plotting and Programming in Python](https://swcarpentry.github.io/python-novice-gapminder/index.html) - This lesson is an introduction to programming in Python for people with little or no previous programming experience.
- [Programming with Python](https://swcarpentry.github.io/python-novice-inflammation/) - This Python lesson teaches data analysis using a case study of inflammation in patients who have been given a new treatment for arthritis.
- [R for Reproducible Scientific Analysis](https://swcarpentry.github.io/r-novice-gapminder/) - R is commonly used in many scientific disciplines for statistical analysis. This lesson teaches novice programmers to write modular code and covers best practices for using R for data analysis.
- [Oceanhackweek 2020 recording: Jupyter, NumPy, Pandas, and Matplotlib](https://www.youtube.com/watch?v=CTUAgpvfze0) - As a part of OceanHackWeek 2020, Leticia Portella gave a pre-hackweek tutorial on Jupyter, NumPy, Pandas, and Matplotlib. The Jupyter notebooks are found [here](https://github.com/oceanhackweek/ohw-preweek/tree/master/data-analysis-modules).

## Conda and installing Python and R environments

### Overview

The Hub is pre-configured with a customized "environment" of Python and R packages designed to run all the tutorial notebooks, and supporting a broad range of oceanographic applications. This environment is created and managed using the open-source [**Conda** package and environment management system](https://docs.conda.io) for installing multiple versions of software packages together with their dependencies, and convenient switching between environments. 

### What is Conda?
[**Conda**](http://conda.pydata.org/docs/) is an **open source `package` and `environment` management system for any programming languages, but very popular among the Python community,**

Conda runs on Windows, macOS, and Linux: *"Conda quickly installs, runs, and updates packages and their dependencies. Conda easily creates, saves, loads, and switches between environments on your local computer. It was created for Python programs but it can package and distribute software for any language."*

For Python, the advantage of conda compared to `pip` is that it has a built in environment management system as well as the management of binaries, and non-Python dependencies.

### Conda on the JupyterHub

The JupyterHub has both a pre-configured base environment, and environments that you create and manage yourself.

#### JupyterHub base environment

The Conda environment for the base JupyterHub environment is defined in [oceanhackweek/jupyter-image](https://github.com/oceanhackweek/jupyter-image/). This image contains hopefully everything you will need for the tutorials and for general exploration.

The [environment.yml](https://github.com/oceanhackweek/jupyter-image/blob/master/environment.yml) captures the current state of the OceanHackWeek environment. You can explore this file to see what packages we have selected to come in the base environment.

```yaml
# environment.yml
name: OHW
channels:
  - conda-forge
dependencies:
  - python=3.9
  - pangeo-notebook=2021.07.24
  - argopy
  - bokeh
  - bottleneck
  - cartopy
  - cdsapi
  - cf-units
  - cf_xarray
  - cmip6_preprocessing
  - cmocean
  - colorcet
  - compilers
  - compliance-checker
  - conda-lock
#   ... oh so many more packages that we are not going to include them all here
```

It also contains a lot of supporting infrastructure for running each individual's JupyterLab server (for instance `compilers` and `conda-lock` in just that small subset), so we suggest building up an environment from scratch, rather than by trimming down the base environment.

The exact state of the Conda environment is captured in [`conda-linux-64.lock`](https://github.com/oceanhackweek/jupyter-image/blob/master/conda-linux-64.lock), which will also include lots of packages that we didn't explicitly select, but are needed dependencies of those we did.

There are also a handful of dependencies that are installed directly in the [Docker image](https://github.com/oceanhackweek/jupyter-image/blob/master/Dockerfile), like RStudio, and the Bigelow Labs R libraries ([`ohwobpg`](https://github.com/BigelowLab/ohwobpg) and [`rasf`](https://github.com/BigelowLab/rasf)).

#### Temporary packages

You can temporarily add packages to your hub, via Jupyter cell magic, `%pip install <list-of-packages>` or `%conda install <list-of-packages>`. In R you can use `install.packages("package-name")` as usual.

!!! Warning

    For those who know their way around Jupyter, you may be tempted to `!pip install <list-of-packages>`. This can leave your environment in an inconsistent state, which may prevent your server from starting (and will require some heavy duty assistance from `@help-infrastructure` to debug). More information is [available here.](https://pilot.2i2c.org/en/latest/admin/howto/environment.html#temporarily-install-packages-for-a-session)

#### Create your own environment on JupyterHub

To create your own Conda environment on JupyterHub, you can launch the terminal and run `conda create` commands as expected. Be sure to specify `-n <environment-name>`. For a Python environment:

`conda create -n cool-project -c conda-forge python=3.9 xarray ipykernel`

Once you've created an environment, you can run `conda activate cool-project` as usual for access to the environment in the terminal. Additionally the environment will become available as a notebook environment if you install `ipykernel` for Python or `irkernel` for R.

!!! Info

    It may take a minute or two for JupyterLab to show your new Conda environment.
    The [package](https://github.com/Anaconda-Platform/nb_conda_kernels) that detects additional environments doesn't run constantly, so give it a second before worrying that you created an environment wrong.

### Conda on your own computer

Conda may be used on your computer as well as the Hub. If you wish to install the same environment as the hub is running, after you install Conda, you can download the [`environment.yml`](https://github.com/oceanhackweek/ohw20-tutorials/blob/master/environment.yml) that we use, then `conda create -n <ENV NAME> --file environment.yml`

#### Installing Conda

There are a few different ways to install conda:

- The [Anaconda Individual Edition](https://www.anaconda.com/products/individual) which comes with a large pre-packaged environment, and a snazzy management interface to help explore what packages are available and what environments you have installed.
- [Miniconda](https://docs.conda.io/en/latest/miniconda.html) is a stripped down version with just the installer, which is really for kick starting other environments.
- There is also [Mamba](https://mamba.readthedocs.io/en/latest/index.html) which is a newer take on Conda that tends to be faster, though it's still under heavy development (and it's what we're actually using).

We recommend the use of Miniconda.

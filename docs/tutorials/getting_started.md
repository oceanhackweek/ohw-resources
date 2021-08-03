# Getting started on tutorials

## Introduction

Tutorials will be run live as Jupyter notebooks on the [OceanHackWeek JupyterHub ("The Hub"), {{ hackweek.jupyterhub_url }}]({{ hackweek.jupyterhub_url }}) in your browser. The instructor and all participants can be running their own copies of the notebooks in their Hub account, with files cloned from the OHW source in GitHub.

Below are instructions for getting the tutorials started on the the Hub in your browser, and updating the tutorials files with the latest version from GitHub. 

The schedule of tutorials is available [here](../schedule.md#main-virtual-event), and links to tutorial materials and some background resources will be available there as well.

## How do I get the tutorial repository into the Hub?

For the tutorials, we recommend the use of [nbgitpuller](https://jupyterhub.github.io/nbgitpuller/) to clone and pull the tutorial repository, [https://github.com/oceanhackweek/ohw-tutorials](https://github.com/oceanhackweek/ohw-tutorials), or update the clone you already have. Use [this magical nbgitpuller link](https://ohw.pilot.2i2c.cloud/hub/user-redirect/git-pull?repo=https%3A%2F%2Fgithub.com%2Foceanhackweek%2Fohw-tutorials&urlpath=lab%2Ftree%2Fohw-tutorials%2F&branch=master) to accomplish this clone or update.

See this [extended discussion](../prep/jupyterhub.md#how-do-i-get-the-tutorial-repository) for more details about `nbgitpuller` and the alternative approach relying on `git` commands and `GitHub` workflows.


<!-- ## Start the Hub in your browser

### Step 1
Navigate to the [OceanHackWeek Hub, {{ hackweek.jupyterhub_url }}]({{ hackweek.jupyterhub_url }}).

### Step 2
Sign in using your GitHub account, if you are not already signed in. We need to have your GitHub account name ("handle") in advance in order to grant you access to the OHW cloud computing environment.

## Upload (`git clone`) a copy of the `oh20-tutorials` GitHub repository and follow along
This basic workflow allows you to follow along with tutorials with your own live copy of the tutorials notebooks while staying up-to-date with any changes made to the master tutorials repository, [ohw20-tutorials](https://github.com/oceanhackweek/ohw20-tutorials).

### Shortcut
The first time you try to upload (`git clone`) the `ohw20-tutorials` repository, launch a new terminal, then enter:

```bash
git clone https://github.com/oceanhackweek/ohw20-tutorials.git
```

Now you have a new `ohw20-tutorials` directory under your "home" directory, `/home/jovyan`. You're good to go!

### Longer description - Step 1
Navigate to the [tutorial repository on GitHub](https://github.com/oceanhackweek/ohw20-tutorials).

Clone the tutorial to the Hub environment. You can easily copy the link to a repository by selecting the green "clone or download" dropdown (making sure the pop up says "Clone with HTTPS") and hitting the clipboard icon, which will automatically copy the link for you.

Launch a terminal using the "plus" sign in the upper left corner of your JupyterHub:

![Jupyter Launch Terminal](../img/Jupyter-LaunchNewTerminal.jpg)

then execute the `git clone` statement:

```bash
git clone https://github.com/oceanhackweek/ohw20-tutorials.git
```

A new `ohw20-tutorials` directory will be created, holding the repository clone.

### Step 2
Follow along by opening and running the tutorial notebooks. You can save changes within your clone (such as edits to a notebook) or add other files, then download a copy to your local machine if you'd like.

### Step 3
Update your Hub copy with any changes to the `origin` repository. If you have saved changes within your local copy of the notebook or added other files, this may cause conflicts (*ask us questions if you run into problems!*). Fetch and merge (using `git pull`) the latest changes from the `origin` remote.

```bash
git pull origin
```

These instructions assume you're working on the default `master` branch.

**Please note: the OceanHackWeek JupyterHub (the Hub) should not be relied upon to save your files beyond the duration of the hackweek, and will be removed a couple of weeks after the hackweek. Thus, for any non-repository changes or repository changes that have not been pushed to GitHub, you MUST complete Step 3 to save the files to your local machine if you would like continued access to them.** 
-->

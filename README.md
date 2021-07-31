# OceanHackWeek learning resources and preliminary tutorials site

OceanHackWeek, [https://oceanhackweek.github.io/ohw-resources](https://oceanhackweek.github.io/ohw-resources)

## Technical notes and instructions for site development

This documentation is built and deployed using [MkDocs](https://www.mkdocs.org/), and uses the markdown extension [admonition](https://squidfunk.github.io/mkdocs-material/extensions/admonition/) and the markdown plugin [markdownextradata](https://github.com/rosscdh/mkdocs-markdownextradata-plugin/). The organization of pages on this site is specified in the `mkdocs.yml` file, together with other site configurations.
  
* Install `mkdocs` and the markdown plugin from `conda-forge`: `conda install -c conda-forge mkdocs mkdocs-markdownextradata-plugin`
* To develop locally, activate the conda environment then run `mkdocs serve` to view and evaluate your edits on your browser
* To publish your edits to the GitHub repository, please use the Git Forking workflow:
  1. Fork this repository
  2. Clone your fork: `git clone https://github.com/mygithubname/ohw-resources.git`
  3. Add the "upstream" (main) GitHub repository as a git remote called "upstream": `git remote add upstream https://github.com/oceanhackweek/ohw-resources.git`
  4. Make your edits locally to the markdown documents, then push your changes to your GitHub fork ("origin"): `git push origin mylocalbranchname`
  5. Submit a Pull Request (PR) from your GitHub fork to the `master` branch of the main repository (the master branch will be selected by default)
* Your proposed changes will be reviewed by [Emilio Mayorga](https://github.com/emiliom) or another person before merging into the `master` branch or asking you via GitHub discussions for clarifications or changes. Once the PR is merged, the web pages will be generated automatically and updated on the `gh-pages` branch. It typically takes a couple of minutes after merginng the PR before the updates are published and visible.

**Note:** You'll find most `MkDocs` instructions pointing to the use of the command `mkdocs gh-deploy` to publish your local edits to the GitHub repository (more specifically, to the `gh-pages` branch). Please ignore those instructions and follow the Git Forking workflow instructions listed above.

## Contributing single-page edits

The easiest way to contribute additions or changes to an existing Learning Resources page, is to go to the page at the web site itself (not the GitHub repository markdown file). That way you can first read it exactly as intended, plus you can find it easily if you start at the `OceanHackWeek Resources` home page. Then click on the "Edit on GitHub" link at the upper right, and edit away. A Pull Request will be generated that will be reviewed by us before "merging" it (your changes) into the repository or asking for clarifications.

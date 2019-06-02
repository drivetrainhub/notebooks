# Contributing
---

Introduction to [open source contribution process](https://github.com/Roshanjossey/first-contributions).

Below are resources to help you contribute code to the Drivetrain Hub Notebook Series.

### Open Issue
---

Before spending the effort on developing code, please open an issue for discussion with moderators:

> Search the GitHub issues in the relevant repository to see if the issue is already identified.  If not found, submit a new issue.

For issues specific to a notebook, go to the issues of the corresponding repository:

- [Issues for notebooks-gears](https://github.com/drivetrainhub/notebooks-gears/issues)
- [Issues for notebooks-fundamentals](https://github.com/drivetrainhub/notebooks-fundamentals/issues)

For high-level issues, such as suggesting a new technical category, see [notebooks issues](https://github.com/drivetrainhub/notebooks/issues).

### Develop Code
---

1. Setup your local development environment:
    1. Upon creating your fork, clone, and branch, you are ready to develop.  [See guide](https://github.com/Roshanjossey/first-contributions#fork-this-repository) for help on this step.
    2. [Pipenv](https://docs.pipenv.org/) for package management and virtual environment.
    3. Run the Jupyter notebook server in your virtual environment: `jupyter notebook`
2. Create or open the notebook you are contributing to.
    1. If creating a new notebook, first discuss your plan with the moderators by opening a GitHub issue.
    2. If creating a new notebook, please use the [notebook template](https://github.com/drivetrainhub/notebooks/blob/master/template.ipynb) to get started.
3. Develop the notebook with clean formatting and proper references.
    1. When including images, it is recommended to save a local copy of the image into an `img` folder in the same directory as the notebook.
    2. Manually add or update the table of contents.  We prefer not to rely on notebook extensions at this time.
    3. To hide certain notebook cells when converted to HTML for online viewing, use these conventions:
        1. Cell tags are used for this functionality, see dropdown View --> Cell Toolbar --> Tags
        2. To hide the cell input, add tag:  hide_input
        3. To hide the entire cell, add tag:  hide_cell
    4. To convert a notebook to HTML, run `nbconvert` from the command line in the notebook directory.  For example:
        ```
        jupyter nbconvert "Chapter 1 - Involute.ipynb" --TagRemovePreprocessor.remove_input_tags="{'hide_input'}" --TagRemovePreprocessor.remove_cell_tags="{'hide_cell'}"
        ```

> TIP #1: If making use of imported Python modules that you are actively developing for use in a notebook, check out the [Jupyter %autoreload command](https://ipython.readthedocs.io/en/stable/config/extensions/autoreload.html?highlight=autoreload#autoreload).  **Only use %autoreload during development, then disable or remove it before submitting a pull request.**

> TIP #2: Need to create an illustration?  We recommend [Inkscape](https://inkscape.org/) for drawing high quality 2D graphics.  Our preferred colors when not using black:  gray (#a7a7a7ff), blue (#006fe1ff), orange (#fc7500ff), pink (#fc00c3ff).

### Pull Code to GitHub
---

1. Ready to merge your code with the GitHub master branch?
    1. Is your notebook using our template format for the header, title, author, and table of contents?
    2. Is your code cleanly formatted and free of typos?
    3. Is your table of contents updated?
    4. Is your code pushed to *your* forked `origin` on GitHub?  [See guide](https://github.com/Roshanjossey/first-contributions#push-changes-to-github) for help.
2. Submit a pull request to the relevant repository:
    1. [Pull request for notebooks-gears](https://github.com/drivetrainhub/notebooks-gears/pulls)
    2. [Pull request for notebooks-fundamentals](https://github.com/drivetrainhub/notebooks-fundamentals/pulls)
    3. Need help?  See [GitHub help on pull requests](https://help.github.com/articles/about-pull-requests/)

### Questions or Inquiries
---

If you found a bug or want to propose edits or additions, follow our [guidelines on opening an issue](#Open-Issue).

For general questions or comments about our Notebook Series, email [code@drivetrainhub.com](mailto:code@drivetrainhub.com)

# Contributing to pygeofilter

We welcome contributions to pygeofilter, in the form of issues, bug fixes, documentation or suggestions for enhancements. This document sets out our guidelines and best practices for such contributions.

It's based on the [Contributing to pygeoapi](https://github.com/geopython/pygeoapi/blob/master/CONTRIBUTING.md) guide which is based on the [Contributing to Open Source Projects
Guide](https://contribution-guide-org.readthedocs.io/).

pygeofilter has the following modes of contribution:

- GitHub Commit Access
- GitHub Pull Requests

## Code of Conduct

Contributors to this project are expected to act respectfully toward others in accordance with the [OSGeo Code of Conduct](https://www.osgeo.org/code_of_conduct).

## Submitting Bugs

### Due Diligence

Before submitting a bug, please do the following:

* Perform __basic troubleshooting__ steps:

    * __Make sure you're on the latest version.__ If you're not on the most
      recent version, your problem may have been solved already! Upgrading is
      always the best first step.
    * [__Search the issue
      tracker__](https://github.com/geopython/pygeofilter/issues)
      to make sure it's not a known issue.

### What to put in your bug report

Make sure your report gets the attention it deserves: bug reports with missing information may be ignored or punted back to you, delaying a fix.  The below constitutes a bare minimum; more info is almost always better:

* __What version of Python are you using?__ For example, are you using Python 3.8+, PyPy 2.0?
* __What operating system are you using?__ Windows (7, 8, 10, 32-bit, 64-bit), Mac OS X,  (10.7.4, 10.9.0), GNU/Linux (which distribution, which version?) Again, more detail is better.
* __Which version or versions of the software are you using?__ Ideally, you've followed the advice above and are on the latest version, but please confirm this.
* __How can the we recreate your problem?__ Imagine that we have never used pygeofilter before and have downloaded it for the first time. Exactly what steps do we need to take to reproduce your problem?

## Contributions and Licensing

### Contributor License Agreement

Your contribution will be under our [license](https://github.com/geopython/pygeofilter/blob/main/LICENSE) as per [GitHub's terms of service](https://help.github.com/articles/github-terms-of-service/#6-contributions-under-repository-license).

### GitHub Commit Access

* Proposals to provide developers with GitHub commit access shall be raised on the pygeofilter [discussions page](https://github.com/geopython/pygeofilter/discussions). Committers shall be added by the project admin.
* Removal of commit access shall be handled in the same manner.

### GitHub Pull Requests

* Pull requests may include copyright in the source code header by the contributor if the contribution is significant or the contributor wants to claim copyright on their contribution.
* All contributors shall be listed at https://github.com/geopython/pygeofilter/graphs/contributors
* Unclaimed copyright, by default, is assigned to the main copyright holders as specified in https://github.com/geopython/pygeofilter/blob/main/LICENSE

### Version Control Branching

* Always __make a new branch__ for your work, no matter how small. This makes it easy for others to take just that one set of changes from your repository, in case you have multiple unrelated changes floating around.

    * __Don't submit unrelated changes in the same branch/pull request!__ If it is not possible to review your changes quickly and easily, we may reject your request.

* __Base your new branch off of the appropriate branch__ on the main repository:

    * In general the released version of pygeofilter is based on the ``main`` (default) branch whereas development work is done under other non-default branches. Unless you are sure that your issue affects a non-default branch, __base your branch off the ``main`` one__.

* Note that depending on how long it takes for the dev team to merge your
  patch, the copy of ``main`` you worked off of may get out of date!
    * If you find yourself 'bumping' a pull request that's been sidelined for a while, __make sure you rebase or merge to latest ``main``__ to ensure a speedier resolution.

### Documentation

* documentation is managed in `docs/`, in reStructuredText format
* [Sphinx](https://www.sphinx-doc.org) is used to generate the documentation
* See the [reStructuredText Primer](https://www.sphinx-doc.org/en/master/usage/restructuredtext/basics.html) on rST markup and syntax


### Code Formatting

* __Please follow the coding conventions and style used in the pygeofilter repository.__
* pygeofilter follows the [PEP-8](http://www.python.org/dev/peps/pep-0008/) guidelines
* 80 characters
* spaces, not tabs
* pygeofilter, instead of PyGeoFilter, pygeoFilter, etc.


#### **pre-commit**
The project is using [`pre-commit`](https://pre-commit.com) to automatically run code formatting and type checking on new commits. Please install `pre-commit` and enable it on your environment before pushing new commits.

```bash
# Install pre-commit
pip3 install pre-commit

# Enable pre-commit
cd /pygeofilter
pre-commit install

# Optional - run pre-commit manually
pre-commit run --all-files
```

## Suggesting Enhancements

We welcome suggestions for enhancements, but reserve the right to reject them if they do not follow future plans for pygeofilter.

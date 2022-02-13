# Dobrev on Read the Docs


## Introduction

[Read the Docs](https://readthedocs.org/) is a managed platform for building and hosting documentation. It's based on [Sphinx](https://www.sphinx-doc.org/) - a doc generator built with Python and launched in 2008.

Docs are loaded from GitHub and can be written in either [reStructuredText](https://docutils.sourceforge.io/rst.html) or [Markdown](https://www.markdownguide.org/).


## Local Setup
1. Clone this repo.
2. Ensure you have [Python 3](https://docs.python.org/3/using/index.html) and [pip](https://pip.pypa.io/en/stable/installation/) installed.
3. Install the dependencies:
```
pip install -r requirements.txt
```
4. Install the neat Read the Docs theme:
```
pip install sphinx-rtd-theme
```


## Building the Docs

**Locally**

1. Build with make:
```
cd docs && make html
```

2. Once the HTML is generated you can open it in the browser:
```
open build/html/index.html
```

**Remotely**

Read the Docs triggers a new build for:
* every merge into the main branch
* every new Pull Request

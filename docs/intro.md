# Books with Jupyter 2.0

```{warning}
This is an early prototype tool that may evolve quickly. Your feedback is
very welcome! To give it, please [open an issue in the CLI repository](https://github.com/ExecutableBookProject/cli/issues/new)
```

This tool provides a command-line interface and a Python API that lets users
do the following:

* Write their content in markdown files, Jupyter Notebooks, or rST files.
* Include computational elements in any of the above (e.g. executable
  code cells along with their outputs)
* Include rich syntax for publication features, such as citations,
  cross-references, and equations.
* Using a simple command, convert this content into:
    * A web-based interactive book
    * A publication-quality PDF

Currently it accomplishes a subset of these features.

## The components of Jupyter Book 2.0

Jupyter Book 2.0 is a wrapper around a collection of tools in the Python
ecosystem that make it easier to publish computational documents. Here are
a few key pieces:

* It uses [the MyST markdown language](https://myst-parser.readthedocs.io/) in
  markdown and notebook documents. This allows users to write rich,
  publication-quality markup in their documents.
* It uses [the MyST-NB package](https://myst-nb.readthedocs.io/) to parse and
  read-in notebooks so they are built into your book.
* It uses [the Sphinx documentation engine](https://www.sphinx-doc.org/en/master/)
  to build outputs from your book's content.
* It uses a slightly-modified version of the [PyData Sphinx theme](https://pandas-sphinx-theme.readthedocs.io/en/latest/)
  for beautiful HTML output.
* It uses a collection of Sphinx plugins and tools to add new functionality.

For more information about the project behind many of these tools, see
[The Executable Book Project](https://ebp.jupyterbook.org/) documentation.


## Get started

To get started, check out the pages above. These are major sections of the documentation.
In particular, {doc}`guide/01_overview` is a good way to get familiar with this tool and how to
create your own books.

## Install

Install this tool directly from the Master branch. When it has stabilized
we will begin creating releases.

```
pip install git+https://github.com/ExecutableBookProject/cli.git@master
```

## Develop

First clone the package:

```
git clone https://github.com/ExecutableBookProject/cli
cd cli
```

Next, install:

```
pip install -e .
```

## Use

The primary way to use this tool is via the command line. It provides a
top-level command called `jupyter-book`, and a number of sub-commands.
Run `jupyter-book -h` for more information.

For more information on how to use this tool, see {doc}`guide/01_overview`.
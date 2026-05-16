# copier-templates

ignition-devs [copier] templates for Ignition projects.

## Pre-requisites

- Git
- [Python 2.7.18] (for `jython` and `python`)
- [Python 3.12] (for [mypy])
- [copier]

  ```sh
    python3 -m pip install copier
  ```

## Templates

### ignition

> [!NOTE]
> This template uses the Ignition [Exchange Resource Style Guide] as reference.

- Automated code checks before committing to version control using [pre-commit]
- Pre-configured tools for code formatting, quality analysis and testing:
  - [coatl-dev/flake8] + [pydoclint]
  - [isort]
  - [pylint]
  - [ruff]
  - [sort-all]
  - [ssort]
  - [unimport]
- Tests run with [sourcery]
- [Python 2.7.18]

### jython

- Automated code checks before committing to version control using [pre-commit]
- Pre-configured tools for code formatting, quality analysis and testing:
  - [black]
  - [coatl-dev/flake8] + [pydoclint]
  - [docformatter]
  - [flake8] (for stubs)
  - [isort]
  - [pydocstyle]
  - [pylint]
  - [sort-all]
  - [ssort]
  - [unimport]
- Tests run with [sourcery], [tox] and [make]
- [Jython 2.7.3], [Python 2.7.18], and [Python 3.12] (for stubs)

### python

- Automated code checks before committing to version control using [pre-commit]
- Pre-configured tools for code formatting, quality analysis and testing:
  - [black]
  - [coatl-dev/flake8] + [pydoclint]
  - [docformatter]
  - [flake8] (for stubs)
  - [isort]
  - [pydocstyle]
  - [pylint]
  - [sort-all]
  - [ssort]
  - [unimport]
- Tests run with [sourcery] and [tox]
- [Python 2.7.18]
- [Python 3.12] (for stubs)

## Quick setup and usage

### Generating a project

You can generate a project from a template using the copier command-line tool:

```sh
copier copy gh:ignition-devs/copier-templates /path/to/destination
```

### Updating a project

Navigate to your project's directory, make sure git status shows it clean, and run:

```sh
copier update --defaults
```

<!-- Links -->
[copier]: https://copier.readthedocs.io/en/stable/
[Exchange Resource Style Guide]: https://files.inductiveautomation.com/ia_exchange/docs/Exchange+Resources+Style+Guide.pdf
[Jython 2.7.3]: https://repo1.maven.org/maven2/org/python/jython-installer/2.7.3/
[Python 2.7.18]: https://www.python.org/downloads/release/python-2718/
[Python 3.12]: https://www.python.org/downloads/latest/python3.12/
<!-- Tools -->
[black]: https://black.readthedocs.io/en/stable/
[coatl-dev/flake8]: https://flake8.pycqa.org/en/5.0.4/
[docformatter]: https://docformatter.readthedocs.io/en/stable/
[flake8]: https://flake8.pycqa.org/en/stable/
[isort]: https://pycqa.github.io/isort/
[make]: https://www.gnu.org/software/make/
[mypy]: https://coatl-mypy.readthedocs.io/en/v0.971/
[pre-commit]: https://pre-commit.com/
[pydoclint]: https://github.com/jsh9/pydoclint
[pydocstyle]: https://coatl-pydocstyle.readthedocs.io/en/latest/
[pylint]: https://pylint.readthedocs.io/en/stable/
[ruff]: https://docs.astral.sh/ruff/
[sort-all]: https://github.com/aio-libs/sort-all
[sourcery]: https://docs.sourcery.ai/
[ssort]: https://github.com/bwhmather/ssort
[tox]: https://tox.wiki/
[unimport]: https://github.com/hakancelikdev/unimport

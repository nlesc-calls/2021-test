# Source files for the call for proposals 2021-test

## Badges

| Description    | Badge |
| ---            | --- |
| metadata       | [![metadata](https://github.com/nlesc-calls/2021-test/actions/workflows/metadata.yml/badge.svg)](https://github.com/nlesc-calls/2021-test/actions/workflows/metadata.yml) |
| convert-to-pdf | [![convert-to-pdf](https://github.com/nlesc-calls/2021-test/actions/workflows/convert-to-pdf.yml/badge.svg)](https://github.com/nlesc-calls/2021-test/actions/workflows/convert-to-pdf.yml) |
| publish        | [![publish](https://github.com/nlesc-calls/2021-test/actions/workflows/publish.yml/badge.svg)](https://github.com/nlesc-calls/2021-test/actions/workflows/publish.yml) |
| Zenodo sandbox | [![DOI](https://sandbox.zenodo.org/badge/DOI/10.5072/zenodo.831247.svg)](https://sandbox.zenodo.org/record/831247) |

## Actions

This project uses the following GitHub Actions:

1. https://github.com/marketplace/actions/cffconvert
1. https://github.com/marketplace/actions/markdown-to-pdf-and-html

## Artifacts

For artifacts, go [here](https://github.com/nlesc-calls/2021-test/actions/workflows/convert-to-pdf.yml).

## Updating the version

We use [`bump2version`](https://pypi.org/project/bump2version/) from PyPI.

```
# make a virtual environment
python3 -m venv env

# activate the environment
source env/bin/activate

# upgrade pip wheel setuptools
pip install --upgrade pip wheel setuptools

# install bump2version
pip install -r requirements.txt

# bumpversion major|minor|patch, e.g.
bumpversion patch

```

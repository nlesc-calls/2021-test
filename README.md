# Source files for the call for proposals 2021-test

## Badges

| Description    | Badge |
| ---            | --- |
| metadata       | [![metadata](https://github.com/nlesc-calls/2021-test/actions/workflows/metadata.yml/badge.svg)](https://github.com/nlesc-calls/2021-test/actions/workflows/metadata.yml) |
| convert-to-pdf | [![convert-to-pdf](https://github.com/nlesc-calls/2021-test/actions/workflows/convert-to-pdf.yml/badge.svg)](https://github.com/nlesc-calls/2021-test/actions/workflows/convert-to-pdf.yml) |
| publish        | [![publish](https://github.com/nlesc-calls/2021-test/actions/workflows/publish.yml/badge.svg)](https://github.com/nlesc-calls/2021-test/actions/workflows/publish.yml) |
| markdown links | [![markdown-link-check](https://github.com/nlesc-calls/2021-test/actions/workflows/markdown-link-check.yml/badge.svg)](https://github.com/nlesc-calls/2021-test/actions/workflows/markdown-link-check.yml) |
| Zenodo sandbox | [![DOI](https://sandbox.zenodo.org/badge/DOI/10.5072/zenodo.831247.svg)](https://sandbox.zenodo.org/record/831247) |

## Actions

This project uses the following GitHub Actions:

1. https://github.com/marketplace/actions/cffconvert
1. https://github.com/marketplace/actions/markdown-link-check
1. https://github.com/marketplace/actions/markdown-to-pdf-and-html

## Artifacts

For artifacts, go [here](https://github.com/nlesc-calls/2021-test/actions/workflows/convert-to-pdf.yml), and click on
the topmost build. On the bottom of the next page, there should be an item named `artifacts`, where you can download a
zip file with the generated `2021-test.pdf` in it.

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

## Publishing

Publish the contents of [`src/2021-test.md`](src/2021-test.md) as a pdf file on Zenodo Sandbox using the [manual workflow
trigger named `publish`](https://github.com/nlesc-calls/2021-test/actions/workflows/publish.yml). Click `Run workflow` to publish.

[![image](https://user-images.githubusercontent.com/4558105/119168638-64c29580-ba61-11eb-8121-d511fc109c30.png)](https://github.com/nlesc-calls/2021-test/actions/workflows/publish.yml)

For more details, see the workflow file [`.github/workflows/publish.yml`](.github/workflows/publish.yml).

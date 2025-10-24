# Knowledge-Base (KB) infrastructure technical notes

## Work environment setup

The repository contains a [pre-commit](https://pre-commit.com/) configuration [file](../.pre-commit-config.yaml) that enforces some basic rules (e.g. validate JSON file syntax, limits on file size). 

After locally cloning the repository, install the git hooks by running `pre-commit install` at the root of the repository.

## Software utilities and configuration

All the software used to manage the KB (data validation, markdown generation and more) is in this repository: https://github.com/IBEXImagingCommunity/ibex_imaging_knowledge_base_utilities

When a new release of the utilities is created, update the url references to the package in the KB GitHub actions, see [.github/workflows](https://github.com/IBEXImagingCommunity/ibex_imaging_knowledge_base/tree/main/.github/workflows) directory.  

The data validation scripts are configurable using JSON files. These are found in the KB [.github/data_validation_configs](https://github.com/IBEXImagingCommunity/ibex_imaging_knowledge_base/tree/main/.github/data_validation_configs) directory.

## Automatic archiving on the Zenodo repository

The KB GitHub repository is [integrated with the Zenodo](https://doi.org/10.5281/zenodo.7693278) generalist data repository. This enables automatic archiving of official KB releases. For details on Zenodo-GitHub integration setup see the [instructions on the Zenodo site](https://help.zenodo.org/docs/github/).

&#x26A0; WARNING

The Zenodo dataset is **automatically** updated when a new release is created on GitHub. Once this happens it cannot be deleted as a DOI is assigned to the data. Make the best possible effort to avoid releases with known issues/errors. If this happens, correct the errors in the GitHub repository and create a new release which will result in a new dataset version on Zenodo (to err is human, to correct said error is science).


## Creating a release

In the local git repository:
1. Checkout the `main` branch and see what tags exist
   ```
   git checkout main
   git tag -n
   ```
2. Create a local tag with the new version, for example v0.5.0 and push the tag to the authoritative remote repository under the IBEXImagingCommunity GitHub organization(code below assumes the remote repository is named `upstream` in your local repository, to check run `git remote -v`) 
```
git tag -a v1.0.0 -m "IBEX Knowledge-Base Release 1.0.0"
git push upstream v1.0.0
```
3. The GitHub actions will automatically create a draft release with release notes enumerating the differences between the current and previous release (e.g. number of new reagent validations, ORCIDs of first time contributors etc.). Edit the notes as appropriate and finalize the release using the GitHub GUI. 

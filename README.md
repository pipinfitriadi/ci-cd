<!--
Copyright (C) Pipin Fitriadi - All Rights Reserved

Unauthorized copying of this file, via any medium is strictly prohibited
Proprietary and confidential
Written by Pipin Fitriadi <pipinfitriadi@gmail.com>, 28 August 2024
-->

# CI/CD

[![License](https://img.shields.io/gitlab/license/pipinfitriadi%2Fci-cd)](LICENSE)

Continuous Integration and Continuous Delivery with GitLab CI

## GitLab CI

Use `jds`'s component in your existing _`.gitlab-ci.yml`_ file to implement [Jabar Digital Service's data product](https://gitlab.com/jdsteam/core-data-platform/data-products/template-data-product) deployment to JabarCloud v1 or JabarCloud v2 (either in the staging or production environment). Please read more in [CI/CD Catalog](https://gitlab.com/explore/catalog/pipinfitriadi/ci-cd).

## Local Development

> [!NOTE]  
> This section only for **INTERNAL DEVELOPER** using Unix-like OS.

Follow these steps the first time you use VS Code after cloning this repository from [GitLab](https://gitlab.com/pipinfitriadi/ci-cd/) or [GitHub](https://github.com/pipinfitriadi/ci-cd):

1. Make sure [Homebrew](https://brew.sh/) is already installed on your computer
2. Make sure [Docker](https://www.docker.com/products/docker-desktop/) is already installed on your computer
3. Create a _`.gitlab-ci-local-variables.yml`_ file based on [_`template.gitlab-ci-local-variables.yml`_](template.gitlab-ci-local-variables.yml) and set your environment values
4. Change the values of the environment variables `LINK_TARGET_DIR`, `GITLAB_CI_LOCAL_CWD`, and `GITLAB_CI_LOCAL_STATE_DIR` in [_`.vscode/tasks.json`_](.vscode/tasks.json)

Whenever you modify and test a GitLab component in [_`templates/`_](templates/) on your computer, use the command <kbd>command</kbd> + <kbd>shift</kbd> + <kbd>P</kbd>, select `Tasks: Run Task`, and then choose `gitlab-ci-local: Run`

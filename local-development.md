<!--
Copyright (C) Pipin Fitriadi - All Rights Reserved

Unauthorized copying of this file, via any medium is strictly prohibited
Proprietary and confidential
Written by Pipin Fitriadi <pipinfitriadi@gmail.com>, 7 October 2024
-->

# Local Development

> [!NOTE]  
> This section only for **INTERNAL DEVELOPER** using Unix-like OS.

Follow these steps the first time you use VS Code after cloning this repository from [GitLab](https://gitlab.com/pipinfitriadi/ci-cd/) or [GitHub](https://github.com/pipinfitriadi/ci-cd):

1. Make sure [Homebrew](https://brew.sh/) is already installed on your computer
2. Make sure [Docker](https://www.docker.com/products/docker-desktop/) is already installed on your computer
3. Create a _`.gitlab-ci-local-variables.yml`_ file based on [_`template.gitlab-ci-local-variables.yml`_](template.gitlab-ci-local-variables.yml) and set your environment values
4. Change the values of the environment variables `LINK_TARGET_DIR`, `GITLAB_CI_LOCAL_CWD`, and `GITLAB_CI_LOCAL_STATE_DIR` in [_`.vscode/tasks.json`_](.vscode/tasks.json)

Whenever you modify and test a GitLab component in [_`templates/`_](templates/) on your computer, use the command <kbd>command</kbd> + <kbd>shift</kbd> + <kbd>P</kbd>, select `Tasks: Run Task`, and then choose `gitlab-ci-local: Run`

---
title: Contributing Code
permalink: /docs/contributing-code/
read_time: true
layout: single
date: Last Modified
sidebar:
  - nav: "universal"
---
# Contributing Code
## Can I Help Fix a Bug?

Sure! 

Have a look at the issue report: if the issue is assigned to someone,
they're on it! Maybe you can find something else to work on, or you can contact 
the person it's assigned to to see if they need a hand.

If the issue is not assigned to anyone, add a comment in the issue indicating 
you'd like to work on resolving the issue and go for it!

## How to Submit Some Code?

Whether you have a fix for an issue, some improved test cases, or a brand
new feature, we welcome your contributions in the form of pull requests.

Your contributions are governed by the [GitHub TOS section 6](https://help.github.com/en/github/site-policy/github-terms-of-service#6-contributions-under-repository-license) which indicate that your contributions are made under the same license as the project.<br><br>Furthermore, by making a contribution to the project, you certify that you have the right to submit to the project as detailed in the [Developer Certificate of Origin](https://developercertificate.org/).{.notice--info}

Follow this process if you'd like your work considered for inclusion in the project:

1. [Fork](http://help.github.com/fork-a-repo/) the project, clone your fork,
   and configure the remotes:

    ```bash
    # Clone your fork of the repo into the current directory
    git clone https://github.com/<your-username>/<repo-name>

    # Navigate to the newly created directory
    cd <repo-name>

    # Assign the repo to a remote called "upstream"
    git remote add upstream https://github.com/<upstream-owner>/<repo-name>
    ```

2. If you cloned a while ago, get the latest changes from upstream:

    ```bash
    git checkout <dev-branch>
    git pull upstream <dev-branch>
    ```

3. Create a new topic branch (off the main project development branch) to
   contain your feature, change, or fix:

    ```bash
    git checkout -b <topic-branch-name>
    ```

4. Commit your changes in logical chunks. Please adhere to these [git commit
   message guidelines](http://tbaggery.com/2008/04/19/a-note-about-git-commit-messages.html). Use Git's
   [interactive rebase](https://help.github.com/articles/interactive-rebase)
   feature to tidy up your commits before making them public.

5. Locally merge (or rebase) the upstream development branch into your topic branch:

    ```bash
    git pull [--rebase] upstream <dev-branch>
    ```

6. Push your topic branch up to your fork:

    ```bash
    git push origin <topic-branch-name>
    ```

7. [Open a Pull Request](https://help.github.com/articles/using-pull-requests/)
   with a clear title and description.

Once submitted, your Pull Request is reviewed and you will receive
some feedback to make sure that it fits in with:

-   the roadmap for the project
-   the architecture of the project
-   the coding [Style Guide](/docs/coding-style-guide/) used by the project

After it has has been accepted, you Pull Request will be merged into the main branch.

Thank you for your contribution!

# Contribution Guidance

If you'd like to contribute to this repository, please read the following guidelines. Contributors are more than welcome to share their learnings with others in this centralized location.

## Question or Problem?

Please do not open GitHub issues for general support questions as the GitHub list should be used for feature requests and bug reports. This way we can more easily track actual issues or bugs from the code and keep the general discussion separate from the actual code.

## Typos, Issues, Bugs and contributions

Whenever you submit any changes to the repositories, please follow these recommendations.

* Always fork the repository to your own account before making your modifications
* Do not combine multiple changes to one pull request. For example, submit any samples and documentation updates using separate PRs
* If your pull request shows merge conflicts, make sure to update your local main to be a mirror of what's in the main repo before making your modifications
* If you are submitting multiple samples, please create a specific PR for each of them
* If you are submitting typo or documentation fix, you can combine modifications to single PR where suitable

## Submitting Pull Requests

Here's a high-level process for submitting new samples or updates to existing ones.

1. Fork this repository [thynclabs/npm-template](https://github.com/thynclabs/npm-template) to your GitHub account
2. Create a new branch from the `main` branch for your fork for the contribution
3. Include your changes to your branch
4. Commit your changes using descriptive commit message * These are used to track changes on the repositories for monthly communications
5. Create a pull request in your own fork and target the `main` branch
6. Fill up the provided PR template with the requested details

Before you submit your pull request consider the following guidelines:

* Search [GitHub](https://github.com/thynclabs/npm-template/pulls) for an open or closed Pull Request
  which relates to your submission. You don't want to duplicate effort.
* Make sure you have a link in your local cloned fork to the [thynclabs/npm-template](https://github.com/thynclabs/npm-template):

  ```shell
  # check if you have a remote pointing to the repo:
  git remote -v

  # if you see a pair of remotes (fetch & pull) that point to https://github.com/thynclabs/npm-template, you're ok... otherwise you need to add one

  # add a new remote named "upstream" and point to the Microsoft repo
  git remote add upstream https://github.com/thynclabs/npm-template.git
  ```

* Make your changes in a new git branch:

  ```shell
  git checkout -b mycustomfunction main
  ```

* Ensure your fork is updated and not behind the upstream **thynclabs/npm-template** repo. Refer to these resources for more information on syncing your repo:
  * [GitHub Help: Syncing a Fork](https://help.github.com/articles/syncing-a-fork/)
  * [Keep Your Forked Git Repo Updated with Changes from the Original Upstream Repo](http://www.andrewconnell.com/blog/keep-your-forked-git-repo-updated-with-changes-from-the-original-upstream-repo)
  * For a quick cheat sheet:

    ```shell
    # assuming you are in the folder of your locally cloned fork....
    git checkout main

    # assuming you have a remote named `upstream` pointing official **thynclabs/npm-template** repo
    git fetch upstream

    # update your local main to be a mirror of what's in the main repo
    git pull --rebase upstream main

    # switch to your branch where you are working, say "mycustomfunction"
    git checkout mycustomfunction

    # update your branch to update it's fork point to the current tip of main & put your changes on top of it
    git rebase main
    ```

* Push your branch to GitHub:

  ```shell
  git push origin mycustomfunction
  ```

<img src="https://telemetry.sharepointpnp.com/powerfx-samples/CONTRIBUTING.md" />

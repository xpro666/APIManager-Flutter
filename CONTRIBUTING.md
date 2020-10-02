# How To Contribute

First off, thank you for considering contributing to `APIManager-Flutter`! It's
people like _you_ who make it such a great tool for everyone.

This document intends to make contribution more accessible by codifying tribal
knowledge and expectations. Don't be afraid to open half-finished PRs, and ask
questions if something is unclear!

## Workflow

- No contribution is too small! Please submit as many fixes for typos and
  grammar bloopers as you can!
- Try to limit each pull request to **_one_** change only.
- Since we squash on merge, it's up to you how you handle updates to the master
  branch. Whether you prefer to rebase on master or merge master into your
  branch, do whatever is more comfortable for you.
- _Always_ add tests and docs for your code. This is a hard rule; patches with
  missing tests or documentation will not be merged.
- You won't get any feedback until and unless you ask for it.
- Once you've addressed review feedback, make sure to bump the pull request with
  a short note, so we know you're done.
- Avoid breaking backwards compatibility.

## Beginner's Guide

This guide is for those who are new to GitHub and Contribution.

- We encourage contribution of all kinds and from anyone willing to contribute,
  even if the contributor is in his/her early stage of learning. So don't
  hesitate to propose your changes.
- Take this small [guide](#working-in-a-forked-project) to configure your repo.
- Create a separate branch for your changes:
  ```
  git checkout -b <your-branch-name>
  ```
- Do your changes and commit on a regular basis:

  - Stage your changes:

    ```
    git add .
    ```

  - Commit your changes:
    ```
    git commit -m "your-commit-message"
    ```

- When you're done with your changes, analyze your code:
  ```
  flutter analyze
  ```
- Finally, if you've followed all the steps correctly you can push your changes:
  ```
  git push origin <your-branch-name>
  ```
- After this you need to create a PR(Pull Request) by following the URL
  generated by the command above.
- If your branch is merged into the original repo's master branch you can then
  update your local repo:

  - To update your local repo, checkout to your master branch:
    ```
    git checkout master
    ```
    After this, you can follow [this guide](#updating-the-forked-repo).

## Working in a forked project

First of all, you need to fork the repo. It will basically create a copy of this
repo in your account.<br> Then you can clone it to your workspace and then
follow [this guide](#adding-upstream-repo).

### Adding upstream repo

- Add the original repo's remote. <br>

  Using https:

  ```
  git remote add upstream https://github.com/101Loop/APIManager-Flutter.git
  ```

  Using ssh:

  ```
  git remote add upstream git@github.com:101Loop/APIManager-Flutter.git
  ```

- Now, that you have added the original repo's remote URL, you can update your
  repo from the original repo.

### Updating the forked repo

The following steps are only necessary for updating your forked repo. If your
forked repo is already even with the original repo, then you don't need to
perform these steps.

**Step 1:** Fetch all the branches of remote upstream.

```
get fetch upstream
```

**Step 2:** Rewrite your master with upstream's master

```
git rebase upstream/master
```

**Step 3:** Finally, push the updates from original repo to your forked repo:

```
git push
```

## Code of Conduct

Please note that this project is released with a Contributor
[Code of Conduct](https://github.com/101loop/APIManager-Flutter/blob/master/CODE_OF_CONDUCT.md).
By participating in this project you agree to abide by its terms. Please report
any harm to `devs [at] 101loop.com` for anything you find appropriate.

Thank you for considering contributing to `APIManager-Flutter`!
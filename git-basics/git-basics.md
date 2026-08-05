## Introduction to Git Version Control

Refer and complete all videos and quizes in [learngit.io](https://learngit.io/)

## Using Remote Repositories

To extend git from local repositories to remote repositories, you need to setup ssh key and configure your git client to use it. This allows you to securely connect to remote repositories hosted on platforms like GitHub, GitLab, or Bitbucket.

Refer to the [GitHub SSH Key Setup Guide](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent) for detailed instructions on generating and adding an SSH key to your GitHub account.

## General Working of Local vs Remote Repositories

![alt_text](images/image-1.png)

Here, are some commands not covered in the above videos and quizzes that you can use to work with remote repositories:

### Cloning a Remote Repository

```bash
git clone <repository-url>
```

This command creates a local copy of a remote repository. Replace `<repository-url>` with the URL of the repository you want to clone.

### Adding a Remote Repository

```bash
git remote add origin <repository-url>
```

This command adds a remote repository to your local git configuration. Replace `<repository-url>` with the URL of the remote repository you want to add.

### Pushing Changes to a Remote Repository

```bash
git push origin <branch-name>
```

This command pushes your local changes to the specified branch of the remote repository. Replace `<branch-name>` with the name of the branch you want to push to.

### Fetching Changes from a Remote Repository

```bash
git fetch origin
```
This command fetches changes from the remote repository without merging them into your local branch. It updates your local copy of the remote branches.

### Pulling Changes from a Remote Repository

```bash
git pull origin <branch-name>
```
This command fetches and merges changes from the specified branch of the remote repository into your local branch

>__NOTE:__ Always run `git fetch` before `git pull` to ensure you have the latest changes from the remote repository.

> Also make it a habit to run `git fetch` and `git pull` EVERYDAY before starting any new work to avoid conflicts and ensure you are working with the most up-to-date code.


### Stashing Changes
```bash
git stash
```
This command temporarily shelves (or stashes) changes you've made to your working directory so you can work on something else, and then come back and re-apply them later on. Useful when you need to switch branches but aren't ready to commit your changes or need to pull updates from the remote repository without losing your current work.

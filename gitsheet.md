#Luis's Git Cheatsheet

### Start a new project

```shell
$ mkdir project_name
$ git init
$ touch readme.md
$ git add readme.md
$ git commit -m "initial commit"
```

### do some work and then save it

First, do some work!

```shell
$ git status
$ git add <whatever file> 
$ git status
$ git commit -m "I made a bunch of changes"
```

### share my work with the world!

First, create a repo via github

```shell
$ git remote add origin git@github.com:<githubusername>/<repositoryname>.git
$ git push -u origin master
```

### Contribute to someone elses's code
First, find the code on github that you want to contribute to

Then Fork it!

```shell
$ git clone git@github.com:<your username>/<repo_name>.git
```

Then, make some changes you think are important.


```shell
$ git add <your files>
$ git commit -m "A very thorough explanation of what we did since this it someone else's work."
$ git push origin master
```

Finish what you started working on, then push any additional commits.

File a pull request with the commits in it that you want to share. Make sure you have a good explanation in the pull request of what this is, what it's intended to do, and some nice language, rather than making fun of the original author.

### Typical collaboration patterns

A typical collaboration pattern is actually to fork, then branch off of master, then push to your fork, then file a pull request.
The reason for this is that master, as a branch, should always represent a code or whatever that "works" and is suitable for deployment or sharing or whatever "going public" is for you.

### Alias homework

```shell
$ git config --global alias.br branch
$ git config --global alias.ci commit
$ git config --global alias.st status
$ git config --global alias.co checkout
```
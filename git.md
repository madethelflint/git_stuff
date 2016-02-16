#Intro to Git
## Rachel Parsons
### @pinkeerach
#### Cardinal Solutions

![inline 100%](CardinalLogo_color.png)

---
## Version Control
### What is it?

System that records changes to files or a set of files over time so that you can recall specific versions later.

---
## Why?
- undo
- experiment
- maintain multiple versions
- blame/credit
- history/accountability
- contribute

^ experiment without impacting working code; blame bugs on commits and prove fixes

---
## Points

- Distributed instead of centralized (SVN, TFS, etc.)
  - No single point of failure
  - Every developer has a full history of the entire project
- Not just for big teams

---

#[fit] Github != git

---

## Installing

```
apt-get install git-core

brew install git

```
[http://git-scm.com/download/win](http://git-scm.com/download/win)

[https://desktop.github.com](https://desktop.github.com)


---

## github

let's go ahead and setup accounts

---

## Common Commands

```
init
clone

add
commit

pull
push
status

checkout
branch
```

---

## More git
### file life cycle

![inline][logo]

[logo]: http://git-scm.com/book/en/v2/book/02-git-basics/images/lifecycle.png "Logo Title Text 2"

---

## More git
### staging and tracked

- File is tracked by running ``` git add ```
  - git is now keeping track of this file
  - .gitignore
- staging
  - ``` git add ```   ....again.....?
  - think of ``` git add ``` as not tracking a file but including it in the next commit

---

## More git
### staging, tracked, and commit

- Skip over staging...
- ``` git commit -a ```
- ``` git commit filename ```
- add -m "your commit message" or let git open your editor

---

## more git
### branching

Current repo

![inline](http://git-scm.com/book/en/v2/book/03-git-branching/images/branch-and-history.png)

---

## create branch for testing

```
git branch testing
```

![inline](http://git-scm.com/book/en/v2/book/03-git-branching/images/head-to-master.png)

---

## checkout branch for testing

```
git checkout testing
```

```
git checkout -b testing
```

![inline](http://git-scm.com/book/en/v2/book/03-git-branching/images/head-to-testing.png)

---

## branch with a commit

```
git commit -am "sample commit message"
```

![inline](http://git-scm.com/book/en/v2/book/03-git-branching/images/advance-testing.png)

---

### let's go back to master

![inline](http://git-scm.com/book/en/v2/book/03-git-branching/images/checkout-master.png)

---

### git
## working with remote

- ``` git fetch ```
  - ``` git merge origin/master ```
- ``` git pull ```
  - merges for you
- ``` git push origin master```

*don't forget to look @ github app*

---

## Walkthrough
### Getting Started

- Desktop app: go to website, click button :)
- CLI: ``` git clone git@github.com:cltmobilemeetup/introductions.git optional_dir_name```
- ``` git log ```
- Open the project using your favorite text editor/IDE

*mention .gitignore*

---
## Walkthrough

### Making changes
- Add your_name.md --- [markdown cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
  - Include your name and a few interesting things about your self
- Add a photo if you want (images directory)

---

## Walkthrough
### Viewing changes

-  ``` git status ```
- ``` git diff ```
- let's look @ github app

---

##github
### pull requests

website and app

readme.md
  - where useful info is stored.
  - setup, license, contributing

contributions.md

---

## Resources

[https://try.github.io](https://try.github.io)

[https://progit.org/](https://progit.org/)

[http://rogerdudler.github.io/git-guide/](http://rogerdudler.github.io/git-guide/)

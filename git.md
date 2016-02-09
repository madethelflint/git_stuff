#Git
## John Hiott
### @johnhiott
#### Cardinal Solutions

---
## Version Control
### What is it?

System that records changes to files or a set of files over time so that you can recall specific versions later.

---
## Why?

- undo a change
- prevent lost code or having a backup that is too old
- maintain multiple versions of a product
- to see the difference between different versions of your code
- prove that a particular change broke or fixed a piece of code
- see the history of some code
- submit a change to someone else's code
- share your code, or let other people work on your code
- see how much work is being done, and where, when and by whom
- experiment with a new feature without interfering with working code

---
## Points

- Distributed instead of centralized (SVN)
  - Not a single point of failure
  - every developer has a full history of the entire project
  - not just for teams
      - github is not git

---

## Installing

```
apt-get install git-core
```

```
brew install git
```

```
https://desktop.github.com
```

---
##Config

```bash
git config --global user.name "Your Name"
git config --global user.email your.email@example.com
```

---
## ssh - optional

```
cd ~/.ssh

ssh-keygen -t rsa -b 4096 -C "your_email@example.com"

pbcopy < my_key.pub

cat my_key.pub
```
---

## Common Commands

```
git init
git clone

git add
git commit

git pull
git push

git diff
git status

git checkout
git branch
```

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
- Add your name as a link to readme.md
- Add a photo if you want (images directory)

---

## Walkthrough
### Viewing changes

-  ``` git status ```
- ``` git diff ```
- let's look @ github app

---

## More git
### staging and tracked

- File is tracked by adding running ``` git add ```
  - git is now keeping track of this file
  - bring up .gitignore again
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

*look @ github app*

---

## More git
### file life cycle

![inline][logo]

[logo]: http://git-scm.com/book/en/v2/book/02-git-basics/images/lifecycle.png "Logo Title Text 2"

---

## more git
### branching

Current repo

![inline](http://git-scm.com/book/en/v2/book/03-git-branching/images/branch-and-history.png)

---
## more git
### branching

create branch for testing

```
git branch testing
```
---

![inline](http://git-scm.com/book/en/v2/book/03-git-branching/images/head-to-master.png)

---
##more git
### branching

checkout branch for testing

```
git checkout testing
```

```
git checkout -b testing
```

---

![inline](http://git-scm.com/book/en/v2/book/03-git-branching/images/head-to-testing.png)

---

## more git
### branching ... with commit

```
git commit -am "sample commit message"
```

---

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

##github
### pull requests

website and app

readme.md
  - where useful info is stored.
      - setup, license, contributing

contributions.md

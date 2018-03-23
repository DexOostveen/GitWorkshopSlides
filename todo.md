class: center, middle

# _Git workshop_ 

???
Some note.


---

class: center, middle

![](https://i.imgur.com/qHtEnDf.jpg)

---

## Commandline

![](http://www.blikoontech.com/wp-content/uploads/2014/02/windowsMingwHelloWorldContents.png)

---

## Commandline

- **$**

--

- **change directory**
```bash
$ cd [foldername]
```
--

- **show directory**
```bash
$ dir
```



---
## INIT

--

- Download en installeer git van https://git-scm.com/downloads.

--

- Regel toegang tot Gitlab.

--

- Configureren naam en email 
```bash
$ git config --global user.email "john.doe@mailhost.com"
$ git config --global user.name "John Doe" 
```

---
## Wat kan je met GIT en waarom zou je het willen gebruiken 
--

-   **historie** 

--

-   **rollback**

--

-   **undo**

--

-   **bug fixing** 

--

-   **branching**

--

-   **samenwerking** 

--

-   **productie vs deployment** 

---

## Globale Werking


--

-   **repository(.git map)**

--

-   **working directory**

--

-   **commit historie schrijven**

--

-   **snapshots**

--

-   **history graph**

![](http://i.stack.imgur.com/OLmxz.png)

---

## Creeer repository
- 
```bash 
$ git init (map naam) 
```
--

- 
```bash
$ git clone [url]
```
--

### Praktijk oefening
--

- 
```bash 
$ git clone http://git.dev.itvitae.nl/dex.oostveen/GitWorkshopProject.git 
```
---

## Info

--

- **commit historie**
```bash
$ git log
$ git log --pretty=oneline
$ git log --pretty=oneline --graph
```

--

- **huidige status**
```bash
$ git status
```

--

- **zie wijzigingen**
```bash
$ git diff
```

--

- **test run**
```bash
$ git [command] --dry-run
```

--

- **help**
```bash
$ git [command] -h
```

---

## Staging

--

- **tracked vs untracked**

--
- 
```bash
$ git add [filename|*|*.ext]
```
--

- **.gitignore**

--

### File states


--

- **staged**

--

- **unmodified**

--

- **modified**

---


class: center, middle
<img  src="https://cdn-images-1.medium.com/max/1200/1*5Avk8LW4btU_1BWgsw1Pxw.png"   width="100%">

<!-- <div style="{width= auto}">
![](https://cdn-images-1.medium.com/max/1200/1*5Avk8LW4btU_1BWgsw1Pxw.png)
</div> -->

---

class: center, middle

.center[![](https://git-scm.com/book/en/v2/book/01-introduction/images/areas.png)]


---
## Commit

--

- **command line**

--
```bash
$ git commit
$ git commit -m "comment"
```
--
```bash
$ git add *
$ git commit
=
$ git commit -a
```

--

- **editor**
```bash
$ git config --global core.editor [editor command|notepad|code|vim]
```

---
## Commit guidelines

--

-   **kleine commits**

--

-   **zinige beschrijvingen**

--

-   **korte samenvatting + uitbreiding**

--

-   **Tegenwoordige tijd**

--

-   **issue nummer**

---

## Branching  

--

- **show branches** 
```bash
$ git branch
```

--

- **create branches**
```bash
$ git branch [name]
```

--
- **delete branches**
```bash
$ git branch -d [name]
```

--

- **switch branches**
```bash
$ git checkout [name]
```

---

## Merging

--

- **merge branches**
```bash
$ git checkout master
$ git merge topic
```

--

- **merge conflicts**
```bash
<<<<<<<<<<<<<< master
code on master branch
==============
code on topic branch
>>>>>>>>>>>>>> topic
```

--

- **commit merge**
```bash
$ git add *
$ git commit -m "merge commit"
```
---
name: branch-model
## Branching Model

---
template: branch-model
### master and development
.scale.center[ 
    ![](http://nvie.com/img/main-branches@2x.png)
     ]
 
---

template: branch-model
### feature
.scale.center[ 
    ![](http://nvie.com/img/fb@2x.png)
]

---

name: sync
## Synchronisatie

---
template: sync

### remotes

--

- **show remotes**
```bash
$ git remote
$ git remote -v #verbose
```

--

- **add remotes**
```bash
$ git remote add [name] [url]
$ git remote add origin "www.github.com/user/project.git"
```

--

- **inspect remote**
```bash
$ git remote show [name] 
``` 

---

template: sync
 

### fetch

--

- fetch
```bash
$ git fetch [remote] # remote is optional
$ git fetch origin
```

--

- merge 
```bash
$ git merge origin/master
```

---
![](https://git-scm.com/book/en/v2/images/remote-branches-2.png)

---
![](https://git-scm.com/book/en/v2/images/remote-branches-3.png)

---

template: sync

### pull

```bash
$ git pull origin master # git pull [remote] [branch]
=                        # default to origin and current branch respectively
$ git fetch
$ git merge origin/master
```
---

template: sync

### push

```bash
$ git push
$ git push [remote] [branch]
$ git push origin master 
```

---

name: workflow
## Workflow

---

template: workflow
### start

--

- **init**
```bash
$ git init [folder]
$ cd [folder]
```

--

- **link existing repository**
```bash
$ git remote add origin [url]
$ git push -u origin master
```

--

- **clone**
```bash
$ git clone [url]
$ cd [folder]
```

---

template: workflow

### edit
<!-- edit
status
stage
status
commit -->

```bash
$ edit file.txt             # modify file
$ git status                # see that file is changed
$ git add [file.txt|*]      # stage file
$ git status                # see that file is staged
$ git commit -m "msg"       # commit changes
$ git status                # see that file is now unmodified
$ git log --pretty=oneline  # see new commit
```

---

template: workflow

### sync
 
```bash
$ git fetch                 # get new commit from server if any
$ git status                # check if there are new commits
$ git pull                  # integrate new commits
# if merge conflict resolve it
$ git status                # check that they are integrated
$ git log pretty=oneline    # see new commit in history
$ git push                  # send new local commit to server
$ git status                # check that 
```

---

## Gitlab

_**git.dev.itvitae.nl**_


_**www.gitlab.org**_

---

## Basis Commandos

- [**git status**](https://www.git-scm.com/docs/git-status)
- [**git log**](https://www.git-scm.com/docs/git-log)
- [**git diff**](https://www.git-scm.com/docs/git-diff)


- [**git init**](https://www.git-scm.com/docs/git-init)
- [**git clone**](https://www.git-scm.com/docs/git-clone)


- [**git add**](https://www.git-scm.com/docs/git-add)
- [**git commit**](https://www.git-scm.com/docs/git-commit)


- [**git checkout**](https://www.git-scm.com/docs/git-checkout)
- [**git branch**](https://www.git-scm.com/docs/git-branch)
- [**git merge**](https://www.git-scm.com/docs/git-merge)


- [**git push**](https://www.git-scm.com/docs/git-push)
- [**git fetch**](https://www.git-scm.com/docs/git-fetch)
- [**git pull**](https://www.git-scm.com/docs/git-pull)


---

## Verder Informatie

### Refrences documenation
- https://git-scm.com/docs/
- https://git-scm.com/docs/giteveryday

### Tutorials
- https://www.atlassian.com/git
- https://try.github.io/
- https://learngitbranching.js.org/
 
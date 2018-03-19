
class: center, middle
# _Git workshop_ 

???
Some note.


---
## INIT

--

- Download en installeer git van www.git-scm.com.

--

- Regel toegang tot Github/Gitlab.

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
- 
```bash
$ git clone [url]
```
### Praktijk oefening
- 
```bash 
$ git clone https://github.com/DexOostveen/GitWorkshop.git 
```
---

## Info
- **commit historie**
- git log
- **huidige status**
- git status
- **zie wijzigingen**
- git diff

---

## Staging

--

- **index**

--

- **tracked vs untracked**

--
- 
```bash
$ git add [filename|*|*.ext]
```
--

- **.gitignore**

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

- **command line**
```bash
$ git commit -m "comment"
```

- **editor**
```bash
$ git config --global core.editor [editor command|notepad|code|vim]
```

---
## Commit guidelines:

-   **kleine commits**

-   **zinige beschrijvingen**

-   **korte samenvatting + uitbreiding**

-   **present tense**

-   **issue nummer**

---

## Branching  

- **show branches** 
```bash
$ git branch
```
- **create branches**
```bash
$ git branch [name]
```
- **switch branches**
```bash
$ checkout [name]
```
---

## Merging

- **merge branches**
```bash
$ git checkout master
$ git merge topic
```

- **merge conflicts**
```bash
<<<<<<<<<<<<<< master
code on master branch
==============
code on topic branch
>>>>>>>>>>>>>> topic
```

- **commit merge**
```bash
$ git add *
$ git commit -m "merge commit"
```

---

## Synchronisatie
<!-- remotes -->
<!-- add remotes -->
<!-- server/master vs origin/master vs master -->


---

## Workflow
### start
init of clone

### edit
edit
status
stage
status
commit

### sync
fetch
status
pull
status
push
status


---

## Gitlab

_**www.git.dev.itvitae.nl**_


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

### Tutorials
- https://www.atlassian.com/git
- https://git-scm.com/docs/giteveryday

!todo
- trygit
- learn git branching
- git documentatie
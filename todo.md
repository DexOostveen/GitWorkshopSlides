
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

- Configuur naam en email

```bash
git config --global user.email "john.doe@mailhost.com"

git config --global user.name "John Doe"
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
git init (map naam) 
```

- 
```bash
 git clone [url]
```
### Praktijk oefening
- 
```bash 
git clone https://github.com/DexOostveen/GitWorkshop.git 
```

---

## Staging

--

- **tracked vs untracked**
--

- 
```bash
git add [filename|*|*.ext]
```
--
 
.center[![](https://git-scm.com/figures/18333fig0201-tn.png)]
<!-- ![](https://git-scm.com/book/en/v2/book/01-introduction/images/areas.png) -->

---

## Commit

```bash
git commit -m "comment"
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
git branch
```
- **create branches**
```bash
git branch [name]
```
- **switch branches**
```bash
checkout [name]
```
---

## Merging

- **merge branches**
```bash
git checkout master
git merge topic
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
git add *
git commit -m "merge commit"
```


---

## Synchronisatie
<!-- remotes -->
<!-- add remotes -->
<!-- server/master vs origin/master vs master -->

<!-- push -->
<!-- fetch -->
<!-- pull -->

---

## Workflow
<!-- init of clone -->
<!-- edit -->
<!-- status -->
<!-- stage -->
<!-- status -->
<!-- commit -->
<!-- log -->
<!-- fetch -->
<!-- status -->
<!-- pull -->
<!-- status -->
<!-- push -->
<!-- status -->
---

## Gitlab

_**www.git.dev.itvitae.nl**_

---

## Basis Commandos

- **git status**
- **git log**


- **git init**
- **git clone**


- **git add**
- **git commit**


- **git checkout**
- **git branch**
- **git merge**


- **git push**
- **git fetch**
- **git pull**


---

## Verder Informatie

- https://www.atlassian.com/git

!todo
- trygit
- learn git branching
- git documentatie
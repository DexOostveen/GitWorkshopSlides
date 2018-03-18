
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

-   **.git map**

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

## Praktijk oefening
-   git clone https://github.com/DexOostveen/GitWorkshop.git 

---

## Creeer repository
- ```bash 
git init (map naam) 
```
- ```bash
 git clone [url]
```
---

## Staging
<!-- tracked vs untracked -->
<!-- unmodified modified staged -->
<!-- todo:plaatje toevoegen  -->
<!-- git add [filename|*|*.ext] -->
---

## Commit
<!-- git commit -m "comment" -->
<!--  -->
---
## Commit guidelines:
-   **kleine commits**
-   **zinige beschrijvingen**
-   **korte samenvatting + uitbreiding**
-   **present tense**
-   **issue nummer**


---

## Branching and Merging
<!-- show branches -->
<!-- create branches -->
<!-- switch branches  checkout-->
<!-- merge branches -->
<!-- merge conflicts -->
---

## Synchronisatie
<!-- remotes -->
<!-- add remotes -->
<!-- server/master vs origin/master vs master -->

<!-- push -->
<!-- fetch -->
<!-- pull -->

---
<!-- 
## GIT Basics
-   **info**
-   **wijziging opslaan**
-   **branching**
-   **sync**
--- -->

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
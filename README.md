# Git / GitHub for development basics

Git:

- _distributed_ version control system
- originally authored by Linus (of Linux fame)
- UNIX philosophy of many small chainable tools

Github:

- online hosting for git repositories
- CI, issues, merging, forking, releases, remote

## Why are Git / Github important for development?

- Contributing to open source
- Literacy
- Bug finding
- Code health

## What is distributed version control?

![Diagram showing that distributed version control users all have a copy of the repository, versus centralized where only one copy exists on the server](https://www.thatcompany.com/wp-content/uploads/2020/03/art3.jpg)

<details>
  <summary>Pros</summary>
  
  * Redundancy
  * Independent working
  * Local = fast
  * Offline
</details>

<details>
  <summary>Cons</summary>
  
  * Stale checkouts
  * Manual merging
</details>

## Some basic terminology

_Github_ is a **remote**, which hosts the remote **repo**. The act of creating your local checkout is called **cloning**. **Commits** are changesets. When you and someone else have conflicts, **merging** creates a commit to resolve those conflicts. When you **rebase**, you temporary remove your commits, update or **fast-forward** the **branch** they're on, and re-apply your commits.

# Exercise

## Installing Git

Ubuntu

```
sudo apt install git-all
```

More info [here](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)

## Getting Started

```
git clone git@github.com:cti-one/git-demo.git
```

## High level workflow

1. Get most recent changes

```
git pull --rebase
```

A regular pull:  
![Diagram showing commits for a regular pull from git](https://git-scm.com/book/en/v2/images/basic-rebase-2.png)  
A rebase pull:  
![Diagram showing commits for a regular pull from git](https://git-scm.com/book/en/v2/images/basic-rebase-3.png)  
2. Commit changes

```
git commit -m 'message'
```

3. Push changes

```
git push
```

## What's next?

- Communication
- Feature branching (optional)
- Use the [organization](https://github.com/CTI-One), email me for help

## Further Reading

- [Basic branching and merging](https://git-scm.com/book/en/v2/Git-Branching-Basic-Branching-and-Merging)
- [Feature branching](https://docs.gitlab.com/ee/gitlab-basics/feature_branch_workflow.html)

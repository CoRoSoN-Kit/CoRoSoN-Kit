# Contribution FAQ (Frequently Asked Questions)

This document is intended to answer questions from (potentially new) contributors for all.
Do you have a question which is not answered here? Feel free to [open an issue](https://github.com/bruno-robot/bruno-robot/issues/new) about it.

## Working with GIT & GitHub is new to me. How to start?

### Workflow

As a first step, it is recommended to understand the typical `git` commands, such as `clone`, `commit`, `push`, `merge`...
As a first step, it is recommended to understand the typical terms, such as clone, commit, push, pull request, ... understand.
Additionally, you should know what `feature branches` are and what `pull requests` are needed for.
There are uncountable tutorials about this, IMHO a nice one is [this one](https://soshace.com/understanding-the-git-workflow/), but any other is definitely okay too.

Regarding the process in this project, we are working with `feature branches`.
This means we do not make commits directly in the main branch.
Every change, no matter how small, is made in a branch created for this purpose and transferred to the main branch via a pull request.
This ensures that everything we publish has been checked by at least 2 people.
It also distributes knowledge and guarantees that there are at least 2 people to contact on this topic from now on.

A typical development process is therefore:

1. A problem, an idea, a feature request, or something similar arises in the form of an issue.
2. Possible solutions and actions are discussed there.
3. A person who wants to take on this task will communicate this in the issue and will be assigned to it.
4. The changes are developed in a separate branch.
   * They consist of at least one, but often several commits.
5. The developer makes a pull request to ask for the changes to be incorporated into main.
6. The changes are reviewed by a reviewer.
   * Does this fix the issue and can be closed?
   * Were all style rules followed?
   * Are the changes traceable and are they sensibly documented?
7. *Optional: If there are change requests by the reviewer, they will be discussed and submitted by the developer.*
8. The changes are merged and are in the main branch.
9. The issue is closed and the feature branch is deleted.

### Tools

There are countless tools to use git, many just use the command line, but there are also nice graphical user interfaces.
[Here's](https://git-scm.com/downloads/guis) a nice list.
Often git is also integrated in the development environment.
For example, with [Visual Studio Code (vscode)](https://code.visualstudio.com/).
The GIT integration in vscode becomes really powerful with the following plugins [^IMHO_tknobi]:

* [GitLens — Git supercharged](https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens)
* [Git Graph](https://marketplace.visualstudio.com/items?itemName=mhutchie.git-graph)

[^IMHO_tknobi]: Note: Personal opinion from tknobi, feel free to use the tools you love.

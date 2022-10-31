# Contribution FAQ (Frequently Asked Questions)

This document is intended to answer questions from (potentially new) contributors for all.
Do you have a question which is not answered here? Feel free to [open an issue](https://github.com/CoRoSoN-Kit/CoRoSoN-Kit/issues/new) about it.

## Repo/Folder structure

```text
coroson-kit
├───src        // software
│   ├───<component>
├───hw         // hardware/pcb designs
│   └───<component>
├───doc        // documentation
|   ├───README.md
│   └───<component>
├───dep        // dependencies/libs
├───samples    // minimal sample code
├───test       // unit/integration tests
└───tools      // additional tooling like bash scripts
```

## Software and tools needed / recommended

We strive to use open source software and tools as much as possible. This is not only because we believe in open source, but also because it makes it easier for everyone to contribute.

### Git

See [Git tooling](#git-tooling)

### PCB design / EDA

We use [KiCad](https://kicad.org/) for PCB design.

### 3D design / CAD

TBD
Probably [FreeCAD](https://www.freecadweb.org/) or Fusion 360 due to its popularity and availability of a free license for students/hobbyists.

### Code editor / IDE

[Visual Studio Code](https://code.visualstudio.com/) is recommended for most tasks. It is free, open source and available for all major operating systems. Additionally, it has a large number of extensions to support virtually any programming language.

## A job failed after my commit / pull request 😮

First of all, don't feel bad if a job fails after your changes.
Believe me, happens to everyone, all the time 😉.
If you click on the small red cross, you will get information about which job failed and why.

### "Lint Codebase" fails

We use the [super-linter](https://github.com/github/super-linter), which bundles different linters, depending on the file type.
To find and fix the problem, you can either commit changes and wait for the job or install the linter locally and fix the problem there before committing.

#### Linting Markdown files

When documenting with Markdown, [markdownlint](https://github.com/igorshubovych/markdownlint-cli) is used.
When using the highly recommended [Visual Studio Code (vscode)](https://code.visualstudio.com/) editor, you can install it as a [plugin](https://marketplace.visualstudio.com/items?itemName=DavidAnson.vscode-markdownlint).
After that you see Markdown errors directly in the "PROBLEMS" section of vscode.

#### Linting text

[textlint](https://textlint.github.io/) is used to lint written text.
There is also a [vscode plugin](https://marketplace.visualstudio.com/items?itemName=taichi.vscode-textlint) here, but the setup was not straight-forward, so I skipped the local installation.

### "Check Links" failed

Nobody likes broken links, so we use a GitHub action to check all links.
See the job details to see the broken link and adjust it.

## Working with GIT & GitHub is new to me. How to start?

### Workflow

As a first step, it is recommended to understand the typical `git` commands, such as `clone`, `commit`, `push`, `merge`...
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
4. The changes are developed in a separate branch and/or fork.
   - They consist of at least one, but often several commits.
5. The developer makes a pull request to ask for the changes to be incorporated into main.
6. The changes are reviewed by a reviewer.
   - Does this fix the issue and can be closed?
   - Were all style rules followed?
   - Are the changes traceable and are they sensibly documented?
7. _Optional: If there are change requests by the reviewer, they will be discussed and submitted by the developer._
8. The changes are merged into the upstream main branch.
9. The issue is closed and the feature branch is deleted.

### Git tooling

There are countless tools to use git, many just use the command-line, but there are also nice graphical user interfaces.
[Here's](https://git-scm.com/downloads/guis) a nice list.
Often git is also integrated in the development environment.
For example, with [Visual Studio Code (vscode)](https://code.visualstudio.com/).
The GIT integration in vscode becomes really powerful with the following plugins [^imho_tknobi]:

- [GitLens — Git supercharged](https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens)
- [Git Graph](https://marketplace.visualstudio.com/items?itemName=mhutchie.git-graph)

[^imho_tknobi]: Note: Personal opinion from tknobi, feel free to use the tools you love.

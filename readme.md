# Git

### What is version control?

Version control is a class of systems responsible for managing changes to computer programs, documents, large websites, 
or other collections of information.

Some examples include...
* Drafts of a book
* Stages of a drawing
* Stages of Software being developed
* A holiday itinerary 

### What is git and how does it work?

Git is a tool used as a version control system. It is a fantastic way for developers to track any changes in their code
base while working on it as a team simultaneously without interfering with each other's work.

Git works by creating snapshots of files at various points in time. These snapshots are referred to as commits which are
stored a local repository. When working together on a remote repository developers can create pull requests to add to
what could be considered the main file. Other contributors will get the chance to review the new changes being proposed
and can create a merge if they agreed on the changes which will change the version of the main file.

### Showcase the basic git command flow. Explain what each command does and showcase the expected output:

* git init - creates an empty Git repository
![git init.png](..%2F..%2F..%2F..%2F..%2FPictures%2Fgit%20init.png)
* git status - displays the state of the working directory
![git status.png](..%2F..%2F..%2F..%2F..%2FPictures%2Fgit%20status.png)
* git add - adds the content of the specified file to the staging state
![git add.png](..%2F..%2F..%2F..%2F..%2FPictures%2Fgit%20add.png)
* git commit - captures a snapshot of the project's currently staged changes
![git commit.png](..%2F..%2F..%2F..%2F..%2FPictures%2Fgit%20commit.png)

### Showcase what `git log` and `git diff` do

#### git log
Lists the commits made in that repository in reverse chronological order
![git_log.png](..%2F..%2F..%2F..%2F..%2FPictures%2Fgit_log.png)

#### git diff
Helps you see, compare, and understand changes in your project

Here's an example:

$ git diff file1.txt
file1.txt
- It contains some text.   (This line was removed)
+ It now contains updated text.   (This line was added)

This code will compare what changes have occurred in file1.txt


### What is `.gitignore` and why should we use it? 

.gitignore is a command that allows us to hide files of our choosing from being detected/mentioned by git.

This is a useful command because...
* It allows you to hide files that could be accidentally added to the repo
* It can let you hide anything that is private
* Reduce clutter

### Distributed Version Control

#### Centralised VC
![centralised VC.png](..%2F..%2F..%2F..%2F..%2FPictures%2Fcentralised%20VC.png)

Source code is stored in a central server maintained by a single authority. Developers check out the code they need to 
work on and make changes directly to that codebase. Once the changes are made, they commit the code back to the central 
server.

#### Distributed VC
![distibuted VC.png](..%2F..%2F..%2F..%2F..%2FPictures%2Fdistibuted%20VC.png)

Distributed version control is similar but addresses some of the limitations of centralised version control. It allows 
developers to create local copies of the code repository, complete with the entire history. Each developer has a full 
copy of the repository on their local machine, including the change history.

### What is GitHub

GitHub is a platform that allows developers to create, store, manage and share their code. It uses Git 
software, providing the distributed version control of Git

### What are some examples of other options/competitors?

* GitLab
* Bitbucket
* OneDev
* Gogs
* Codeberg

### How do you link a local repo to a remote repo on GitHub?

![connecting a local repo to a new remote repo.png](..%2F..%2F..%2F..%2F..%2FPictures%2Fconnecting%20a%20local%20repo%20to%20a%20new%20remote%20repo.png)

As can be seen by the image above I'm linking my git_learning local repo to the remote repo I created on GitHub

### How do you link a remote repo to a new local repo? 

To do this you first need to create a remote repo and have the relevant link that is created alongside that.
![git link.png](..%2F..%2F..%2F..%2F..%2FPictures%2Fgit%20link.png)

You then need to run the command in the bash terminal as seen below...
````
git clone <github link/url>
````
You now need to navigate to the new local repo (using the cd command) that has been cloned from the github repository.

It's then possible to create a new folder for example and use the command git init to create a new local repo

You are now free to continue working within that repo making changes and then commit/push items to the remote repo as
with the previous method.


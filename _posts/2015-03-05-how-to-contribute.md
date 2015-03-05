---

layout: post
title:  "note updates"
date:   2015-03-05
categories: announcements 

---


### Instructions to do contribute/modify the repository

(instructions lifted from [https://github.com/maxlieblich/etalecohomology/blob/master/instructions.md](https://github.com/maxlieblich/etalecohomology/blob/master/instructions.md))

In order to follow these instructions, you should have git installed on your local computer

**STEP 1**:
First go to https://github.com/ and create a github account.

**STEP 2**:
Now navigate to [https://github.com/dkrashen/csa/](https://github.com/dkrashen/csa/)
and locate the button in the upper right hand corner called Fork.  Click
the button to create a fork.  This should create a new repository on the
github server called https://github.com/<your username>/csa/

**STEP 3**:
Next, we want to clone the current repository (meaning get a copy on our
local computer).  To do this, 
open a terminal and type

```
git clone https://github.com/<your username>/csa.git

```
This should create a directory on your local computer called csa.

**STEP 4**:
Inside the directory csa, change what you feel like changing! You can't hurt anything from your computer.

**STEP 5**:
If you made changes to any files, made new files, or deleted old files, you
need to tell the git repository (ie. stage the changes).  For example, if
you edited or created the file unicorns.md and deleted the file
vampires.md, you should run the commands

```  
git add unicorns.md
git del vampires.md
```

If you forgot what files you changed, you can view this by running the
command

```
git status
```

Changes that are staged to be committed to the repository and changes which
haven't been will be explained by the output.

**STEP 6**:
When you are satisfied with your contribution, you should make a pull
request.  To do this, you should first 
commit your changes to the local repository.  This is done with the command

```
git commit -m "This is my message about what changes I made"
```

Then you should push your changes to the remote repository.  This is done
via the command


```
git push origin master
```


Finally, you should submit a pull request by navigating to
https://github.com/<your username>/csa
and clicking the green button.

from here, I'll have the option to review your changes and integrate things into the class repository.

NOTES:
You may occasionally want to update your fork of the repository with the
trunk.  This is done via the commands

```
git fetch upstream
git checkout master
git merge upstream/master
```

You may want to save your work occasionally to the local repository by
running

```
git commit -m "some comment about my latest change"
```

This way if you break something on your local copy, you can go back to a
previous version and try again.



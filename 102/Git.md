# What is Git?

Git is a *Distributed Version Control systems* (DVCS) that stores data in a file system made up of snapshots. each times you save changed version of your file
called **commit**, Git creates a snapshot of the file and stores a reference to it.

Git mostly relies on local operations because most necessary information can be found in local resources.Every single change applied to any file or directory is tracked by Git. And, as the gatekeeper, Git will always detect file corruption or loss of information in transit.

Files in Git can reside in three main states: committed, modified and staged.

*Committed*
Data is securely stored in a local database

*Modified*
File has been changed but not committed to the database

*Staged*
Flagged a file’s changed version to be committed in the next snapshot

![states](https://blog.udemy.com/wp-content/uploads/2015/08/image066.png)

After installing Git, users should immediately set the user name and email address, which will be used for every Git commit.

```
git config --global user.name "Jane Smith"

git config --global user.email "example@email.com"
```

To import an existing project or directory into Git, follow these steps using the Terminal or Command Line:
1. Switch to the target project’s directory
```
$ cd test (cd = change directory)
```
2. Use the git init command
```
$ git init
```
3. To start tracking these repository files, perform an initial commit by typing the following:
```
$ git add *.c
$ git add LICENSE
$ git commit -m “any message here”
```
Now, your files are tracked and there’s an initial commit

You can also create a copy of an existing Git repository from a particular server by using the clone command with a repository’s URL:
```
$ git clone https://github.com/test
```
By cloning the file, you have copied all versions of all files for a project. This command leads to the creation of a directory called “test,” with an initialized .git directory inside it, which has copies of all versions of all files for the specified project

To clone a repository into a directory with another name of your choosing, use the following command format:
```
$ git clone https://github.com/test mydirectory
```

The local Git repository has three components:
1. Working Directory: the actual files resides here.
2. Index : the area used for staging.
3. Head : points to the most recent commit.

All files in a working copy of a project file are either in a tracked or untracked state.

***Tracked***
Tracked files can be modified, unmodified, or staged; they were part of the most recent file snapshot.

***Untracked***
Untracked files were not in the last snapshot and do not currently reside in the staging area.


**The life cycle of file status**:
1. After you edit a file, Git flags it as **modified** because of changes made after the previous commit.
2. You stage the modified file.
3. Then, you commit staged changes.

![stages](https://blog.udemy.com/wp-content/uploads/2015/08/image006.png)

**Tracking and Staging a New File**
To track a single file use the following format:
```
git add filename
```
and you can track all files in a repository by using the following command:
```
$ git add *
```

After using these commands, files are tracked and staged for committing.


**Committing a File**
After staging one or multiple files, you should commit the changes and record what you did within the commit message:
```
$ git commit -m “made change x,y,z”
```
also you can commit all modifications of tracked files in the working directory:
```
$ git commit -a
```

Next, you would push changes to a remote repository.
```
$ git push origin master
```


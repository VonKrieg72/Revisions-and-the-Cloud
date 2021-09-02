# Revisions-and-the-Cloud

## Version Control

**Version Control** is a system that enables you to revisit various versions of a file, or set of files by making a record of changes. Through Version Control, you can change a file back to a previous version of itself, track modifications and modifying individuals and compare changes. 

**Local Version Control System** (Local VCS) was created many years ago by programmers, and it has one database on your hard disk, that stores changes to files.

**Centralized Version Control System** (CVCS) was created due to multiple people on development teams needing to collaborate on a single file or set of files. 

However, CVS had many drawbacks. For example, If a CVS were to go down, collaborators wouldn't be able to work with each other on a file, or save changes and new versions. Also, if the central database's hard disk were to be corrupted without any backups, all work would be lost, with the exception of portions on a local machine. 

In response to these short comings, **Distributed Version Control Systems** (DVCS) was created. In DVCS, programmers working together on a team were able to prevent the loss of data, by enabling them to create mirrored repositories, which served as data backups, that could be easily placed on the server to replae any lost information. 

## So What is Git

Git is a DVCS that stores data in a file system made up of snapshots. Snapshots of files are created by Git, and the references are stored. Whenever you make changes to a project and change it, it's called a commit. Because a project's hstory resides on a local disk, Git relies on local operations, which enables it to process things with expedience. Git tracks every single change made to a file, and always detects file corruption or loss of information in transit, because of this, permanent damage to files is greatly minimized. Git has three main states:

Committed- Data is securely stored in a local databse. 

Modified- File has been changed, but not committed to the database.

Staged- Flagged a file's changed version to be committed in the next snapshot. 

## Getting Started

There are three ways to install Git on your computer:

Install it as a package

Install it via another installer

Download and compile the source code

On Windows, Mac, Linux Os you can download from the Git Website 

[(http://git-scm.com/download/windows)]   /mac  /linux

You can download from Github on Mac and Windows 

[(http://mac.github.com)]. [(http://windows.github.com)]

## Initial Customizations

After installing Git, it's recommended to perform customization steps, which should only need to be completed once. There's a tool called "Git Config" which allows the setting of configuration variables that control Git's operation and look. You're going to have to set up your user name and email in order to use Git Commit. In order to do so, type the following into your terminal or command line:

git config --global user.name "your name here"

git config --global user.email "example@email.com"

To confirm that the setting are correct, enter the following commands:

git config --global user.name (should return your name)

git config --global user.email (should return example@email.com)

Git will use the system's default text editor, unless you choose to configure a different text editor. For example, if you choose to use emacs as a text editor you have to install it. Enter the following command into the terminal command line:

git config --global core.editor emacs

In the event that you need help, there's three commands you can enter:

git help command

git command --help

man git-command

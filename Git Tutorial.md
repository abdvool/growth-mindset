# Git 


## Prerequisites
Before beginning this tutorial, it is highly recommended that you have a solid understanding of the Terminal (for Mac) or Command Line (for Windows and Linux).

## Version Control
Version Control is a system that allows you to revisit various versions of a file or set of files by recording changes. Through version control, one can revert a file or project to a previous version, track modifications and modifying individuals, and compare changes. By utilizing a Version Control System (VCS), mistakes with files can easily be rectified.



## So, what is Git?
* **Snapshots**

Git is a DVCS that stores data in a file system made up of snapshots. Each time you save a changed version of your project — called commit — Git creates a snapshot of the file and stores a reference to it. If the file has not changed, Git only stores a reference to the already-stored identical version of it.

* **Local Operations**

Git mostly relies on local operations because most necessary information can be found in local resources. This allows for process expediency because a project’s history resides on the local disk, eliminating the need to fetch history information from the server, and allowing one to continue work on a project even when not online or on a VPN.

* **Tracking Changes**

Every single change applied to any file or directory is tracked by Git. And, as the gatekeeper, Git will always detect file corruption or loss of information in transit.

* **Loss of Data**

Git is set up to greatly minimize the possibility of irreversible damage to files, such as accidentally lost data. Git makes it extremely difficult for a snapshot of your file that is committed to be lost.

* **States**

Files in Git can reside in three main states: committed, modified and staged.

* **Committed**

Data is securely stored in a local database

* **Modified**

File has been changed but not committed to the database



## How to save your work at Github when you finish?

### Here are  the 3  simple steps to do :



1.  **git add . (with space)** : when I do some changes on my file I use git add . or instead of . I can add the file name itself, but we use . as a shortcut to stage the changes in all files and folders in my repo

2.  **git commit -m 'the message you want'** (the msg should be between ' ' or " ") : to commit my changes

3.  **git push origin main ** : in order to have my changes on GitHub (on the cloud) I use git push origin main,
You will be asked to provide your username and password of your GitHub account






# GIT PAGE 


## **Version Control**

a system that allows you to revisit various versions of a file or set of files by recording changes.

 Through version control:

 *one can revert a file or project to a previous version

 *track modifications and modifying individuals, and compare changes. 

 *By utilizing a Version Control System (VCS), mistakes with files can easily be rectified.


### **what is Git?**

Each time you save a changed version of your project — called commit — Git creates a snapshot of the file and stores a reference to it. If the file has not changed, Git only stores a reference to the already-stored identical version of it.


* Git mostly relies on **local operations** because most necessary information can be found in local resources. This allows for process expediency because a project’s history resides on the local disk, eliminating the need to fetch history information from the server, and allowing one to continue work on a project even when not online or on a VPN.

#### **how it help**

* Tracking Changes

Every single change applied to any file or directory is tracked by Git. And, as the gatekeeper, Git will always detect file corruption or loss of information in transit.

* Loss of Data

Git is set up to greatly minimize the possibility of irreversible damage to files, such as accidentally lost data. Git makes it extremely difficult for a snapshot of your file that is committed to be lost.



**Files in Git can reside in three main states: committed, modified and staged.**

* Committed

Data is securely stored in a local database

* Modified

File has been changed but not committed to the database

* Staged

Flagged a file’s changed version to be committed in the next snapshot

![image to explain](https://blog.udemy.com/wp-content/uploads/2015/08/image066.png)


** Setting up a Git Repository **

* $ cd test (cd = change directory)
* git commit -m “any message here”
* git clone https://github.com/test

** sava a change you made from rep to github **

* $ git add *
* Committing a File 
(
$ git commit -m “made change x,y,z”)

* Pushing Changes  

  ($ git commit -m “made change x,y,z”)
 
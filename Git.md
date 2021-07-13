# So, what is Git?
Git is a piece of software that allows you to monitor changes in any group of files. It's typically used to coordinate work among programmers who are working on source code together during software development. Speed, data integrity, and support for dispersed, non-linear processes are among its objectives.
- Snapshots

Git is a distributed version control system (DVCS) that saves data in a snapshot-based file system. Git produces a snapshot of the file and maintains a reference to it every time you commit a modified version of your project. Git only stores a reference to the already-stored identical version of the file if it hasn't changed.

- Local Operations

Because the majority of essential information may be obtained in local resources, Git mostly depends on local activities. Because a project's history is stored on the local disk, it eliminates the need to request information from the server, allowing you to work on a project even while you're not connected to the internet or using a VPN.

- Tracking Changes

Git keeps track of every modification made to any file or directory. Git will always identify file corruption or information loss in transit since it is the gatekeeper.

- Loss of Data

Git is designed to substantially reduce the risk of irreversible file damage, such as data loss due to human error. Git makes it exceedingly impossible for a committed snapshot of your file to be lost.

- States

Git files can be in one of three states: committed, updated, or staged.

Committed

The information is kept safe in a local database.

Modified

The file has been modified, but it has not yet been committed to the database.

________________
## Terminologies
### 1. Graphical User Interface (GUI) (The normal windows screens)
### 2. Command Line Interface (CLI) (The black screen terminal)
### - Commands for the terminal:
#### 1. ls : displays a list of directories (folders) and files for me (That are not hidden)
#### 2. ls -la :  a list of all the files (with hidden ones)
#### 3. cd (Change Directory): to open a certain directory (folder), for instance, cd test -> If I'm in the test directory and want to go back to the previous one (let's say it's named testPrevious), I simply write cd..
#### 4. mkdir (Make directory) is a command that creates a directory (folder) I now have a new directory called newTest thanks to mkdir newTest.
#### 5. pwd (Print Working Directory): to see where I'm at currently 
#### 6. clear : the terminal is cleared
# Version control

1. ## Local Version Control
A Local VCS entails one database on your hard disk that stores changes to files.


2. ## Centralized Version Control
This system entails a single server storing all changes and file versions, which can be accessed by various clients.

3. ## Distributed Version Control
If a CVS goes down, collaborators cannot work with each other on a file or save changes and new versions.
DVCS allows clients to create mirrored repositories. These data backups can be easily be placed on the server to replace any lost information.

# What is Git?
Git is a DVCS that stores data in a file system made up of snapshots. Each time you save a changed version of your project — called commit — Git creates a snapshot of the file and stores a reference to it. If the file has not changed, Git only stores a reference to the already-stored identical version of it. And it works on local operations.

# Getting started 
to start using git you must download it to your computer that fit your operating system. 

# Setting up a Git Repository

### start with cloning your repository by creating a copy of an existing Git repository then using the command:
   * git clone url

# Tracking and Staging a New File
1. single file use this command:
   * git add filename
2. all files
   *  git add *
# Committing a File
you should commit the changes and record what you did within the commit message:
* git commit -m “made change x,y,z”
# Pushing Changes
you would push changes to a remote repository. 
* git push origin master








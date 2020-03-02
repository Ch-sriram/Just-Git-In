# Just Git In
Learn about Git and GitHub step-by-step, with well explained concepts in theory and practice.

Resources
1. [Official Git Documentation](https://git-scm.com/docs)
2. [Jason Taylor's Online Git & GitHub Course](https://www.udemy.com/course/github-ultimate/)

## Table Of Contents
1. [What is Git?]()
2. [What is a Repository?]()
3. [Commits & Snapshots]()
4. [What is GitHub?]()
5. [Git & GitHub Installation]()
6. [The Basics of Git]()
   1. [Making a new git repository (initialization)]()
   2. [Logical States in Git]()
   3. [Commits in Git]()
   4. [Overview of a Git Repository]()
   5. [Initializing a Git Repository w. Existing Files/Project]()
   6. [Commit History w. Log and Show]()
   7. [Express Commits]()


## 1. What is Git?
Git is a fast, scalable, distributed revision control system with an unusually rich command set that provides both high-level operations and full access to internals. 

In simple words, it is basically a system which allows the user/developer to maintain different versions of their softwares/projects across their cloud service (which is GitHub, bitbucket, etc) or in the local machine (using git bash).

Git is super fast because it supports local operations. It means that we can completely work disconnected from the internet. All of the changes made locally, will be pushed onto the remote repository when there's an active internet connection available, automatically.

Git is Open Source and has an extremely active community thereby, finding help/resources related to Git & GitHub is extremely easy.


## 2. What's a Repository?
Repository is a collection of files managed by Git. These collection of files are also managed with their entire history (version, names, etc).

The repository in the local machine is considered as the Working Directory or the Workspace. The Workspace can contain, both files from git and other files and directories related to the project.

Normally, within the root folder of the repo, there's a pseudo-hidden <strong>.git</strong> directory which contains its own collection of files and directories that make up the entire internal structure of the repository. 


## 3. Commits and Snapshots
Git works by saving the current state (state: changes made till now, meaning the current version of the software) of all its files it manages, into <em>snapshots</em> called <strong>Commits</strong>. A commit can contain more than one changes made to the files inside your repository.

Git doesn't version the directories, but only versions the files inside your repository. As we make changes to the state of the repository, the commits are saved onto a timeline known as a <strong>Branch</strong>. 

A git repository will have at least one branch known as the <strong>master</strong> branch. Additional branches can be created, which we will look into later.


## 4. What is GitHub?
GitHub is a git repository hosting service provided by GitHub, Incorporation (owned by Microsoft) at [GitHub.com](https://www.github.com).

There are other hosting services, and one of the popular ones is bitbucket. But GitHub is the most popular git repository hosting service online. GitHub stands out as a git repo hosting service because it provides unlimited free public repositories to be maintained by an individual/organization. It means that as long as you're comfortable with others being able to look into your code, you can have as many public repositories as you want.

Therefore, in order to have private repositories in your GitHub account, you've to pay for the service. Because of this, most of the open source community has adopted GitHub as their main choice for hosting their git repositories. Even the source code git itself is hosted on GitHub.

GitHub also has some additional features such as Issue Tracking, GitHub Webpages, Source Code Snippet Sharing (in the form of <em>gists</em>), etc to support developer projects hosted on GitHub.


## 5. Git & GitHub Installation
Goto: https://git-scm.com/ and follow the instructions there to download Git for an OS. 

After installing Git, open Git Bash and set the username and email using the following command syntax:

<code>git config --global user.name "Your Name"</code>

<code>git config --global user.email "Your Email"</code>

Example:

<code>git config --global user.name "John"</code>

<code>git config --global user.email "john.doe@example.com"</code>


Install P4Merge for Visual Compare and Merge Tool. Download P4Merge from [here](https://www.perforce.com/downloads/visual-merge-tool). Choose the installer that matches your system and download the installer to install P4Merge Visualizer Tool.

After installation, type in the following commands in Git Bash to install P4Merge as the default graphical compare tool.

<code>git config --global diff.tool p4merge</code>

<code>git config --global difftool.p4merge.path "Absolute-Path-To-Where-P4Merge-Is-Installed"</code> (Example: <code>git config --global difftool.p4merge.path "C:/Program Files/Perforce/p4merge.exe"</code>)

<code>git config --global difftool.prompt false</code>

The following commands are used to make P4Merge as the default graphical merge tool using git bash:

<code>git config --global merge.tool p4merge</code>

<code>got config --global mergetool.p4merge.path "Absolute-Path-To-Where-P4Merge-Is-Installed"</code>

<code>git config --global mergetool.prompt false</code>


## 6. The Basics of Git
We will learn how to make new repositories, how to get information/status of a repository, basic workflow of a repository, how to apply file operations like renaming, moving & deleting files in the git repository, excluding unwanted files from the git repository and undoing mistakes.

### 6.1 Making a new git repository (initialization)
To make a new repository in your system, first create a new directory anywhere in your system using <code>mkdir project</code> (let's say we use "project" as the name of the repository).

Then simply inside the "project" directory, we run the <code>git init "repo-name"</code> command, where "repo-name" can be any name you want without the double quotes (ex: <code>git init demo</code>).

### 6.2 Logical States in Git (Local/Remote)
There are 3 local states related to files being managed by git. These three states are:
1. Working Directory.
2. Staging Area.
3. Repository (.git directory) aka Commit History.

The Working Directory contains our application's files and folders, and therefore, git is aware of these files as a logical state known as "Working Directory".

On the other hand, we've the .git folder, where all teh commit history is saved and thereby git knows at as the final state (in local machine) which is the "Repository" state. .git folder contains all the committed and saved changes of the repository. Anything in .git folder is a part of git's history.

In between is the git's Staging Area. This state is used to prepare for the next commit. Files are moved from the modified "Working Directory" state, to the Git "Staging Area" and then finally committed into the Git "Repository". These aforementioned 3 states of git are specific to the local git repository.

Now, even in the remote repository (the same repository which is hosted on GitHub), we have these same 3 states. Conceptually, we can think of the Remote repository as a state in itself, because all the changes made inside the local environment is saved in the cloud, at a remote server, thereby, we are accessing the remote repository.

This is how the files go from one state to another:

Working Directory => Staging Area => Repository (.git folder) => Remote Repository.


### 6.3 Commits in Git
To get the information about a git repository, we can use the <code>git status</code> command. We'll see that (for a newly created repository), we'll have the information related to the branch (which will be <em>master</em>) and the commit message (which will be <em>initial commit</em>).


To commit changes made inside a git repository, we first need to make changes inside the repository. After that, we can save the changes and again type in the  <code>git status</code> command, which will give us the commit we are on (which will be 'initial commit'), and there'll be some <strong>untracked files</strong> (the files that you changed and are not committed in the local repository). Right now, the files are the "Working Directory (modified)" state. Now, if we want to get these modified files in the repository to the "Staging Area" state, we need to type in the  <code>git add &lt;file-name></code> command (example:  <code>git add README.md</code>). 


Now that our file is in the staging area, we can verify that using the  <code>git status</code> command. If we type it, we will see that we are still in the "initial commit" in the master branch, but we'll see that there's some new information which is <strong>Changes to be committed</strong> and git bash will show all the files which are in the staging area which are ready to be committed.


To make sure that the files in the staging area are committed to the repository (.git folder), we give  <code>git commit -m &lt;commit-message></code> command in the git bash where the &lt;commit-message> can be any message depending on the changes made to the repository. When we commit the changes to the repository, we get information about the number of file changes and the number of insertions/deletions with a commit ID (which is a unique hashed value like 7dxc32e).


Now when we type in the  <code>git status</code> command, we get the information that we are still on the master branch and we have nothing to commit in the working directory, which is mentioned as:  <em>nothing to commit, working directory clean</em>.



### 6.4 Overview of a Git Repository
Inside our repository, currently, we have one file (say) which README.md which is committed. Whatever our repository's name is (let's say "demo"), our directory, is the working directory of our git repository. The actual git repository is contained within .git folder which inside our working directory. The .git folder is a special directory that git manages internally.


To get into the .git folder, we have to get into the .git folder using <code>cd .git/</code> command, and when we check the files inside the .git folder using <code>ls -al</code>, we will see that the we will see certain files which are <em>HEAD, branches, config, description, hooks, index, info, logs, objects, refs, etc</em>. These files are not to be changed without the knowledge of how to do so.


To change our working directory into a normal folder, we can simply remove the .git folder from our working directory, and our directory will simply be a normal folder in our filesystem. To remove the .git folder, we type in <code>rm -rf .git</code> command to (-rf: recursively and forcefully) delete anything that's contained inside the .git folder. When we return to our prompt, we can see in the git bash that now, it knows the fact that we are no longer inside a git repository, we are inside a normal directory, and therefore, the git bash won't show any branch information with the directory we are inside. 


If we simply type in <code>git status</code> into the git bash now, git bash will respond with the following message: 

<em>fatal: Not a git repository (or any of the parent directories): .git</em>


### 6.5 Initializing a Git Repository w. Existing Files/Project
Now that we've deleted our .git folder, our "demo" folder is no longer a git repository, therefore, to make it a git repository, we first navigate the git bash to the "demo" folder, and just type in <code>git init .</code> command in the git bash, where . means "current folder". It will initialize the git repository inside the current folder. 

When we type in <code>ls -la</code> in the git bash, we can see that now our "demo" folder contains the .git folder and therefore now our current working directory has become a git repository.

Now we can follow the steps [6.3 Commits in Git]() to make changes and commit the changes in the git repository we created.


### 6.6 Commit History w. Log and Show
Within our "demo" git repository to show all the commits/changes that have been made in our repository (in the order of most recent to least recent), we simply type in <code>git log</code> command and we will get the information about all the commits we have made so far, regarding our git repository. The commits contain the hash identifier (which is a SHA-1 ID to uniquely commits within a repository) along with the Author (which contains the user.name and user.email), Date followed by the commit message. 

We can get a similar information using the <code>git show</code> command. It will show the last commit we made to the repository and a <code>diff</code> containing all the changes we made in the commit. To get out of the <code>show</code> command, we simply press 'q' in the git bash.


### 6.7 Express Commits
Inside git bash, we are in the "demo" git repository. When we type in <code>git status</code> command, we can see that there will be a message - <em>nothing to commit, working directory clean</em>. Inside our "demo" git repo, it shows that we have a LICENCE.md & README.md file. If we update one of them and again type in the <code>git status</code> command in the git bash, we can see that git will show us the message - <strong>modified: &lt;file-name></strong>.

The difference between previous commits and this commit is that this time, the files are not untracked, they're tracked, but modified. This is how git tracks the difference between tracked and untracked files in a git repository. To know the files that are being tracked by git, we type in the <code>git ls-files</code> in the git bash. Git will show all the files that are being tracked by it. Now if we add a new file to the "demo" repository and again when we type in <code>git ls-files</code> command, we can see that git is still not tracking the new file. When we type in the <code>git status</code> command, we will see that there will be 2 messages: <strong>modified: &lt;prev-file></strong> and <strong>Untracked files: &lt;new-file></strong>.

We can get rid of the newly created file using <code>rm &lt;new-file-name></code> and if we again type in <code>git status</code> command, we will see that there will only be one message and it will be the <strong>modified: &lt;file-name></strong>. Now to commit these changes, we can simply type in <code>git commit -m "commit-message"</code> into the git bash. But, we can do something much better by committing the changes expressly. The Express Commits rely upon one thing, which are/is the tracked file(s) in the repository. To add the files to the staging area and then commit them in a single command, we type in <code>git commit -am "commit-message"</code> into the git bash. Here, <code>-am</code> option => a: add all modified and tracked files to the staging area, and m: give the commit with a message. 

When we say we are adding the modified files into the git's staging area, we are basically adding the modifications to the git repository, not the entire modified file.

Now when we type in <code>git log</code> into the git bash, we can see all the commits we made till now and also the most recent commit that we made earlier at the top of the logs.
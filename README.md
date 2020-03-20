# Just Git In

Learn about Git and GitHub step-by-step, with well explained concepts in theory and practice.

## Resources

- [Official Git Documentation](https://git-scm.com/docs)
- [Jason Taylor's Online Git & GitHub Course](https://www.udemy.com/course/github-ultimate/)


## Table Of Contents

1. [What is Git?](https://github.com/Ch-sriram/Just-Git-In#1-what-is-git)
2. [What is a Repository?](https://github.com/Ch-sriram/Just-Git-In#2-whats-a-repository)
3. [Commits & Snapshots](https://github.com/Ch-sriram/Just-Git-In#3-commits-and-snapshots)
4. [What is GitHub?](https://github.com/Ch-sriram/Just-Git-In#4-what-is-github)
5. [Git & GitHub Installation](https://github.com/Ch-sriram/Just-Git-In#5-git--github-installation)
6. [The Basics of Git](https://github.com/Ch-sriram/Just-Git-In#6-the-basics-of-git)
   1. [Making a new git repository (initialization)](https://github.com/Ch-sriram/Just-Git-In#61-making-a-new-git-repository-initialization)
   2. [Logical States in Git](https://github.com/Ch-sriram/Just-Git-In#62-logical-states-in-git-localremote)
   3. [Commits in Git](https://github.com/Ch-sriram/Just-Git-In#63-commits-in-git)
   4. [Overview of a Git Repository](https://github.com/Ch-sriram/Just-Git-In#64-overview-of-a-git-repository)
   5. [Initializing a Git Repository w. Existing Files/Project](https://github.com/Ch-sriram/Just-Git-In#65-initializing-a-git-repository-w-existing-filesproject)
   6. [Commit History w. Log and Show](https://github.com/Ch-sriram/Just-Git-In#66-commit-history-w-log-and-show)
   7. [Express Commits](https://github.com/Ch-sriram/Just-Git-In#67-express-commits)
   8. [Rolling Back Changes](https://github.com/Ch-sriram/Just-Git-In#68-rolling-back-changes)
   9. [Creating New Commands - Git Alias](https://github.com/Ch-sriram/Just-Git-In#69-creating-new-commands---git-alias)
   10. [Renaming & Deleting Files Using Git Bash](https://github.com/Ch-sriram/Just-Git-In#610-renaming--deleting-files-using-git-bash)
   11. [Renaming & Deleting Files Not Using Git Bash, but the OS Commands](https://github.com/Ch-sriram/Just-Git-In#611-renaming--deleting-files-not-using-git-bash-but-the-os-commands)
   12. [Excluding/Ignoring Unwanted Files in our Git Repository](https://github.com/Ch-sriram/Just-Git-In#612-excludingignoring-unwanted-files-in-our-git-repository)
7. [Advanced Version Control Using Git](https://github.com/Ch-sriram/Just-Git-In#7-advanced-version-control-using-git)
   1. [Comparing Differences in Git](https://github.com/Ch-sriram/Just-Git-In#71-comparing-differences-in-git)
   2. [Branching and Merging Types in Git](https://github.com/Ch-sriram/Just-Git-In#72-branching-and-merging-types-in-git)
   3. [Special Markers/Pointers](https://github.com/Ch-sriram/Just-Git-In#73-special-markerspointers)
   4. [Example of Branching](https://github.com/Ch-sriram/Just-Git-In#74-example-of-branching)
   5. [Conflict Resolution While Merging](https://github.com/Ch-sriram/Just-Git-In#75-conflict-resolution-while-merging)
   6. [Marking Special Events w. Tagging](https://github.com/Ch-sriram/Just-Git-In#76-marking-special-events-w-tagging)
   7. [Saving Work in Progress w. Stashing](https://github.com/Ch-sriram/Just-Git-In#77-saving-work-in-progress-w-stashing)
   8. [Time Travel w. Reset & Reflog](https://github.com/Ch-sriram/Just-Git-In#78-time-travel-w-reset--reflog)
8. [Basics of GitHub](https://github.com/Ch-sriram/Just-Git-In#8-basics-of-github)
   1. [Linking to our GitHub Repository (Local <-> Remote)](https://github.com/Ch-sriram/Just-Git-In#81-linking-to-our-github-repository-local---remote)
   2. [Pushing Changes to GitHub (Local to Remote)](https://github.com/Ch-sriram/Just-Git-In#82-pushing-changes-to-github-local-to-remote)
9. [SSH Authentication](https://github.com/Ch-sriram/Just-Git-In#9-ssh-authentication)
   1. [Generating an SSH Key](https://github.com/Ch-sriram/Just-Git-In#91-generating-an-ssh-key)
10. [GitHub Repository](https://github.com/Ch-sriram/Just-Git-In#10-github-repository)
    1. [Cloning a GitHub Repository](https://github.com/Ch-sriram/Just-Git-In#101-cloning-a-github-repository)
    2. [Fetch & Pull in GitHub](https://github.com/Ch-sriram/Just-Git-In#102-fetch--pull-in-github)
    3. [Updating Remote References of a Repository](https://github.com/Ch-sriram/Just-Git-In#103-updating-remote-references-of-a-repository)
    4. [Creating New Files in GitHub on a New Branch](https://github.com/Ch-sriram/Just-Git-In#104-creating-new-files-in-github-on-a-new-branch)
    5. [Synchronizing Changes made in Remote Repository to the Local Repository](https://github.com/Ch-sriram/Just-Git-In#105-synchronizing-changes-made-in-remote-repository-to-the-local-repository)


## 1. What is Git?

Git is a fast, scalable, distributed revision control system with an unusually rich command set that provides both high-level operations and full access to internals. 

In simple words, it is basically a system which allows the user/developer to maintain different versions of their softwares/projects across their cloud service (which is GitHub, bitbucket, etc) or in the local machine (using git bash).

Git is super fast because it supports local operations. It means that we can completely work disconnected from the internet. All of the changes made locally, will be pushed onto the remote repository when there's an active internet connection available, automatically.

Git is Open Source and has an extremely active community thereby, finding help/resources related to Git & GitHub is extremely easy.

[Goto: Table Of Contents](https://github.com/Ch-sriram/Just-Git-In#table-of-contents)

## 2. What's a Repository?

Repository is a collection of files managed by Git. These collection of files are also managed with their entire history (version, names, etc).

The repository in the local machine is considered as the Working Directory or the Workspace. The Workspace can contain, both files from git and other files and directories related to the project.

Normally, within the root folder of the repo, there's a pseudo-hidden <strong>.git</strong> directory which contains its own collection of files and directories that make up the entire internal structure of the repository. 

[Goto: Table Of Contents](https://github.com/Ch-sriram/Just-Git-In#table-of-contents)

## 3. Commits and Snapshots

Git works by saving the current state (state: changes made till now, meaning the current version of the software) of all its files it manages, into <em>snapshots</em> called <strong>Commits</strong>. A commit can contain more than one changes made to the files inside your repository.

Git doesn't version the directories, but only versions the files inside your repository. As we make changes to the state of the repository, the commits are saved onto a timeline known as a <strong>Branch</strong>. 

A git repository will have at least one branch known as the <strong>master</strong> branch. Additional branches can be created, which we will look into later.

[Goto: Table Of Contents](https://github.com/Ch-sriram/Just-Git-In#table-of-contents)

## 4. What is GitHub?

GitHub is a git repository hosting service provided by GitHub, Incorporation (owned by Microsoft) at [GitHub.com](https://www.github.com).

There are other hosting services, and one of the popular ones is bitbucket. But GitHub is the most popular git repository hosting service online. GitHub stands out as a git repo hosting service because it provides unlimited free public repositories to be maintained by an individual/organization. It means that as long as you're comfortable with others being able to look into your code, you can have as many public repositories as you want.

Therefore, in order to have private repositories in your GitHub account, you've to pay for the service. Because of this, most of the open source community has adopted GitHub as their main choice for hosting their git repositories. Even the source code git itself is hosted on GitHub.

GitHub also has some additional features such as Issue Tracking, GitHub Webpages, Source Code Snippet Sharing (in the form of <em>gists</em>), etc to support developer projects hosted on GitHub.

[Goto: Table Of Contents](https://github.com/Ch-sriram/Just-Git-In#table-of-contents)

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

[Goto: Table Of Contents](https://github.com/Ch-sriram/Just-Git-In#table-of-contents)

## 6. The Basics of Git

We will learn how to make new repositories, how to get information/status of a repository, basic workflow of a repository, how to apply file operations like renaming, moving & deleting files in the git repository, excluding unwanted files from the git repository and undoing mistakes.

[Goto: Table Of Contents](https://github.com/Ch-sriram/Just-Git-In#table-of-contents)

### 6.1 Making a new git repository (initialization)

To make a new repository in your system, first create a new directory anywhere in your system using <code>mkdir project</code> (let's say we use "project" as the name of the directory).

Then simply inside the "project" directory, we run the <code>git init "repo-name"</code> command, where "repo-name" can be any name you want without the double quotes (ex: <code>git init demo</code>).

[Goto: Table Of Contents](https://github.com/Ch-sriram/Just-Git-In#table-of-contents)

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

[Goto: Table Of Contents](https://github.com/Ch-sriram/Just-Git-In#table-of-contents)

### 6.3 Commits in Git

To get the information about a git repository, we can use the <code>git status</code> command. We'll see that (for a newly created repository), we'll have the information related to the branch (which will be <em>master</em>) and the commit message (which will be <em>initial commit</em>).


To commit changes made inside a git repository, we first need to make changes inside the repository. After that, we can save the changes and again type in the  <code>git status</code> command, which will give us the commit we are on (which will be 'initial commit'), and there'll be some <strong>untracked files</strong> (the files that you changed and are not committed in the local repository). Right now, the files are the "Working Directory (modified)" state. Now, if we want to get these modified files in the repository to the "Staging Area" state, we need to type in the  <code>git add &lt;file-name></code> command (example:  <code>git add README.md</code>). 


Now that our file is in the staging area, we can verify that using the  <code>git status</code> command. If we type it, we will see that we are still in the "initial commit" in the master branch, but we'll see that there's some new information which is <strong>Changes to be committed</strong> and git bash will show all the files which are in the staging area which are ready to be committed.


To make sure that the files in the staging area are committed to the repository (.git folder), we give  <code>git commit -m &lt;commit-message></code> command in the git bash where the &lt;commit-message> can be any message depending on the changes made to the repository. When we commit the changes to the repository, we get information about the number of file changes and the number of insertions/deletions with a commit ID (which is a unique hashed value like 7dxc32e).


Now when we type in the  <code>git status</code> command, we get the information that we are still on the master branch and we have nothing to commit in the working directory, which is mentioned as:  <em>nothing to commit, working directory clean</em>.

[Goto: Table Of Contents](https://github.com/Ch-sriram/Just-Git-In#table-of-contents)

### 6.4 Overview of a Git Repository

Inside our repository, currently, we have one file (say) which README.md which is committed. Whatever our repository's name is (let's say "demo"), our directory, is the working directory of our git repository. The actual git repository is contained within .git folder which inside our working directory. The .git folder is a special directory that git manages internally.

To get into the .git folder, we have to get into the .git folder using <code>cd .git/</code> command, and when we check the files inside the .git folder using <code>ls -al</code>, we will see that the we will see certain files which are <em>HEAD, branches, config, description, hooks, index, info, logs, objects, refs, etc</em>. These files are not to be changed without the knowledge of how to do so.

To change our working directory into a normal folder, we can simply remove the .git folder from our working directory, and our directory will simply be a normal folder in our filesystem. To remove the .git folder, we type in <code>rm -rf .git</code> command to (-rf: recursively and forcefully) delete anything that's contained inside the .git folder. When we return to our prompt, we can see in the git bash that now, it knows the fact that we are no longer inside a git repository, we are inside a normal directory, and therefore, the git bash won't show any branch information with the directory we are inside. 

If we simply type in <code>git status</code> into the git bash now, git bash will respond with the following message: 

<em>fatal: Not a git repository (or any of the parent directories): .git</em>

[Goto: Table Of Contents](https://github.com/Ch-sriram/Just-Git-In#table-of-contents)

### 6.5 Initializing a Git Repository w. Existing Files/Project

Now that we've deleted our .git folder, our "demo" folder is no longer a git repository, therefore, to make it a git repository, we first navigate the git bash to the "demo" folder, and just type in <code>git init .</code> command in the git bash, where . means "current folder". It will initialize the git repository inside the current folder. 

When we type in <code>ls -la</code> in the git bash, we can see that now our "demo" folder contains the .git folder and therefore now our current working directory has become a git repository.

Now we can follow the steps [6.3 Commits in Git](https://github.com/Ch-sriram/Just-Git-In#63-commits-in-git) to make changes and commit the changes in the git repository we created.

[Goto: Table Of Contents](https://github.com/Ch-sriram/Just-Git-In#table-of-contents)

### 6.6 Commit History w. Log and Show

Within our "demo" git repository to show all the commits/changes that have been made in our repository (in the order of most recent to least recent), we simply type in <code>git log</code> command and we will get the information about all the commits we have made so far, regarding our git repository. The commits contain the hash identifier (which is a SHA-1 ID to uniquely commits within a repository) along with the Author (which contains the user.name and user.email), Date followed by the commit message. 

We can get a similar information using the <code>git show</code> command. It will show the last commit we made to the repository and a <code>diff</code> containing all the changes we made in the commit. To get out of the <code>show</code> command, we simply press 'q' in the git bash.

[Goto: Table Of Contents](https://github.com/Ch-sriram/Just-Git-In#table-of-contents)

### 6.7 Express Commits

Inside git bash, we are in the "demo" git repository. When we type in <code>git status</code> command, we can see that there will be a message - <em>nothing to commit, working directory clean</em>. Inside our "demo" git repo, it shows that we have a LICENCE.md & README.md file. If we update one of them and again type in the <code>git status</code> command in the git bash, we can see that git will show us the message - <strong>modified: &lt;file-name></strong>.

The difference between previous commits and this commit is that this time, the files are not untracked, they're tracked, but modified. This is how git tracks the difference between tracked and untracked files in a git repository. To know the files that are being tracked by git, we type in the <code>git ls-files</code> in the git bash. Git will show all the files that are being tracked by it. Now if we add a new file to the "demo" repository and again when we type in <code>git ls-files</code> command, we can see that git is still not tracking the new file. When we type in the <code>git status</code> command, we will see that there will be 2 messages: <strong>modified: &lt;prev-file></strong> and <strong>Untracked files: &lt;new-file></strong>.

We can get rid of the newly created file using <code>rm &lt;new-file-name></code> and if we again type in <code>git status</code> command, we will see that there will only be one message and it will be the <strong>modified: &lt;file-name></strong>. Now to commit these changes, we can simply type in <code>git commit -m "commit-message"</code> into the git bash. But, we can do something much better by committing the changes expressly. The Express Commits rely upon one thing, which are/is the tracked file(s) in the repository. To add the files to the staging area and then commit them in a single command, we type in <code>git commit -am "commit-message"</code> into the git bash. Here, <code>-am</code> option => a: add all modified and tracked files to the staging area, and m: give the commit with a message. 

When we say we are adding the modified files into the git's staging area, we are basically adding the modifications to the git repository, not the entire modified file.

Now when we type in <code>git log</code> into the git bash, we can see all the commits we made till now and also the most recent commit that we made earlier at the top of the logs.

[Goto: Table Of Contents](https://github.com/Ch-sriram/Just-Git-In#table-of-contents)

### 6.8 Rolling Back Changes

Here, we will back out the changes we made previously by unstaging our changes from the git staging area and then finally we will revert our changes entirely. 

In our "demo" git repository, when we git bash the command <code>git status</code>, we can see that there will be nothing to commit and we will see the following message: <em>nothing to commit, working directory clean</em>.

Now, we will modify the README.md file again and we will put some random text inside it. We save and close the README and then we again type in <code>git status</code> command inside the git bash. We can see that we will have the message - <strong>modified: README.md</strong> and then we can add the changes into the repository using <code>git add .</code> command in our git bash. When we type in <code>git status</code> again, we can see that we see the message - <strong>Changes to be committed: modified: README.md</strong> in the git bash. 

Now, to unstage the changes, or undo the commit, we can type in the command <code>git reset HEAD README.md</code> where README.md is the file to be unstaged from the user's repository. When we open up our README.md file, the changes that we made, will still be there, but the changes that we made have simply been unstaged, that means, when we type in the command <code>git status</code>, we can see that the message we get is - <strong>Changes not staged for commit: modified: README.md</strong> in the git bash.

Now, if we don't want the changes that we made and to discard the changes made to the repository, we can simply revert back to the last known good state (or commit) of the respective file (here, it is README.md) whose details are available inside the .git folder, we simply type in <code>git checkout -- &lt;file-name></code> (ex: <code>git checkout -- README.md</code>). Now, we can check the status of the repository with <code>git status</code> command, which will respond with the message - <em>nothing to commit, working directory clean</em> in the master branch of our "demo" repository. Now if we open README.md, we can see that the changes we made are also gone.

[Goto: Table Of Contents](https://github.com/Ch-sriram/Just-Git-In#table-of-contents)

### 6.9 Creating New Commands - Git Alias

We will create a git alias to shorten a command into a smaller command. In our "demo" repository, in the master branch, when we type in <code>git status</code>, we can see that we have <em>nothing to commit, working directory clean</em> as the message. Now to see the options available with the <code>git log</code> command, we can simply type in <code>git help log</code> command.

Out of all the options available, we can type in the log command as <code>git log --oneline --graph --decorate --all</code> where <strong>--online</strong>: provides a simplified commit entry providing the log information in a single line instead of multiple lines, <strong>--graph</strong>: provides an asterisk(*) based graph denoting our branching hierarchy, <strong>--decorate</strong>: tells us which commits are part of which branches, <strong>--all</strong>: provides the history for all the branches that are available in the repository. We will see an output in git bash which will show us the entire history of our significant commits. Now, whenever we want to get details in this manner, we always have to type in <code>git log --oneline --graph --decorate --all</code> command every time. Instead of typing it all the time, we can use <strong>git aliases</strong>.

To create a git alias (which is basically a new command in git bash and a shortened representation of an existing combination of longer command(s)) we will type in <code>git config --global alias.hist "log --oneline --graph --decorate --all"</code> command in the git bash and we have created an alias for the above command called "hist". So whenever we want to call the longer command, we can simply type in <code>git hist</code>. To check our list of aliases that we have configured in git configuration, we simply type in <code>git config --global --list</code> command in the git bash.

Using aliases, we can also add more options to the underlying command, it simply replaces the alias command with the actual command and concatenates the options that we added. For example, the command <code>git hist -- LICENCE.md</code>, will convert into the actual command which is <code>git log --oneline --graph --decorate --all -- LICENCE.md</code>, where the command will give us all the commit logs related to LICENCE.md file in the repository.

[Goto: Table Of Contents](https://github.com/Ch-sriram/Just-Git-In#table-of-contents)

### 6.10 Renaming & Deleting Files Using Git Bash

In our demo repository, we will create a file called <strong>example.txt</strong> and insert some random text into the file and save and return back to the git bash. We type in <code>git status</code> and check the status of our git repository and we will see the message <strong>Untracked files: example.txt</strong>. We will add the new file using <code>git add example.txt</code> command in git bash. Finally, we commit the changes made into the repo using <code>git commit -m 'adding example.txt'</code>. When we list the files in the git bash using <code>ls -la</code> command, we will see that we have the three files <strong>LICENCE.md, README.md & example.txt</strong> in our repository. 

Now, if we want to change the name of the file we just made, we can change the name in the git bash using the <code>git mv example.txt demo.txt</code> command. When we again check the status of the repository (using <code>git status</code> command), we will see the message - <strong>Changes to be committed: renamed:     example.txt -> demo.txt</strong>. This change is in the staged state. The renaming takes effect properly, only when we commit. When we list the files of the repository (using <code>ls -la</code> command) in git bash, we can see that the file has already been renamed on the Operating System. But to finish the task, we need to actually commit the changes and let our changes be in the .git directory, in the final state, the Committed State. For that, we type in <code>git commit -m "renamed example.txt to demo.txt"</code>. We will see a message - <strong>rename example.txt => demo.txt (100%)</strong> where the 100% inside the parentheses is the confidence level given by git that this file's content is a 100% similar to the previous file name, i.e., example.txt's context hasn't been changed, only the name of the file has been changed to demo.txt. If we would've made modifications to demo.txt before committing the state of the repository, then the confidence level would've been lower than 100%.

If we wanted to delete a file that we made, we can remove it using the <code>rm</code> command in the git bash. To remove it using the git bash (instead of the facilities provided by the OS), we type in <code>git rm demo.txt</code> command in the git bash. If we delete/rename/modify files using the git commands (instead of the commands provided by the OS), we will get the additional benefit of git tracking the changes that we made in our repository. And so, we will have more power with us using the version control system. Now, if we simply list the files in our repository, we will see that we no longer have demo.txt file in our repository. Now, when we check the status of our repository (using <code>git status</code> command), we can see the message - <strong>Changes to be committed: deleted:    demo.txt</strong>, meaning, our deletion is just staged, it hasn't been committed. Therefore, we have to commit to completely reflect the changes in the .git directory of our repository using <code>git commit -m "deleting demo.txt file"</code>. When we check the status of our repo, we should see the message <em>nothing to commit, working directory clean</em>.

[Goto: Table Of Contents](https://github.com/Ch-sriram/Just-Git-In#table-of-contents)

### 6.11 Renaming & Deleting Files Not Using Git Bash, but the OS Commands

We will create a new file in the demo repository using the OS commands (<code>notepad file-name</code> command for Windows Systems and <code>touch file-name</code> command for Linux/Mac Systems). We will list the files using the terminal (<code>dir</code> for Windows systems and <code>ls</code> for Linux/Mac systems). We will rename LICENCE.md to LICENCE.txt using the OS' terminal (Windows: <code>rename LICENCE.md LICENCE.txt</code>, Linux/Mac: <code>mv LICENCE.md LICENCE.txt</code>). Note that we are trying to make new files and rename them using the respective OS' commands and therefore, git sees these changes differently. When we check the status of our repository (using <code>git status</code> command), we will see that we have the message -
<pre>
Changes not staged for commit: 
      <strong>deleted:   LICENCE.md</strong>

Untracked files:
      <strong>LICENCE.txt</strong>
      <strong>myfile.txt</strong>
</pre>

We can see that we see <strong>myfile.txt</strong> as an untracked file. But git sees the renaming of the file using the terminal as a deletion and a new file addition to the repository. Therefore, we need to tell git about our recent changes. To stage the deletions in our repository, we type in <code>git add -u</code> where -u stands for "update". When we check the status of the repository (using <code>git status</code> command), we can see that we have the message -
<pre>
Changes to be committed: 
      <strong>deleted:   LICENCE.md</strong>

Untracked files:
      <strong>LICENCE.txt</strong>
      <strong>myfile.txt</strong>
</pre>

Now, we can see that only the deletions are taken care of. In order to include both additions and deletions in our repository, we have to type in <code>git add -A</code> in the cmd/terminal where -A covers all types of modifications made to the repository (both addition and deletions) properly. Now when we check the status of our repository (using <code>git status</code> command), we will see the message - 
<pre>
Changes to be committed: 
      <strong>renamed:   LICENCE.md -> LICENCE.txt</strong>
      <strong>new file:  myfile.txt</strong>
</pre>

At this point, these changes are only staged. We have to commit the changes using <code>git commit -m "rename and add"</code> command in the cmd/terminal of our pwd. We can check the status after we commit using the <code>git status</code> command.

Now, if we want to delete the <strong>myfile.txt</strong>, we can type in the respective OS' command from the cmd/terminal (Windows: <code>del myfile.txt</code>, Linux/Mac: <code>rm myfile.txt</code>). Now when we check the status of our repository, we will see the message - 
<pre>
Changes not staged for commit: 
      <strong>deleted:   myfile.txt</strong>
</pre>

Now we stage our deletion using <code>git add -u</code> command in the cmd/terminal. Check the status of our repository, and we will see the message - 
<pre>
Changes to be committed: 
      <strong>deleted:  myfile.txt</strong>
</pre>

Now we commit the changes made to the repository using <code>git commit -m "removed myfile.txt"</code> command. When we check the status again, we will see the message - <em>nothing to commit, working directory clean</em>.

[Goto: Table Of Contents](https://github.com/Ch-sriram/Just-Git-In#table-of-contents)

### 6.12 Excluding/Ignoring Unwanted Files in our Git Repository

Assume that we create a new log file inside our demo repository (Windows: <code>notepad app.log</code> & Linux/Mac: <code>touch app.log</code>). When we check the status of the git repository, we will see that the newly created log file is untracked, and the message we should get is - 

<pre>
Untracked files:
      <strong>app.log</strong>
</pre>

In general, in a repository, we don't want anything other than the source code of the app that we are developing. Therefore, log files, images, videos, etc are not supposed to be in our git repository. For this, our version control, i.e., git, has to ignore these files. To exclude files/folders that we don't want in our git repository, we create a <strong>.gitignore</strong> file inside which we write the relative paths of the files that we don't want to be tracked in our repository.

Therefore, we create a <strong>.gitignore</strong> file in cmd/terminal (Windows: <code>notepad .gitignore</code> & Linux/Mac: <code>touch .gitignore</code>) and then type in the relative path of the file/folder that we want to completely exclude from being tracked by the git version control. In our case, we want to exclude app.log file, and therefore, in our .gitignore file, we can type in the following - 

<strong>.gitignore</strong>
<pre>
app.log
</pre>

Otherwise, if we want to exclude all the log files, we can type in the following - 
<strong><em>.gitignore</em></strong>
<pre>
*.log
</pre>

Now, any file that ends with .log extension will be excluded from being tracked in our repository. We can save the .gitignore file and then close the file and in the terminal, we can again check the status of the repository (using <code>git status</code>) and we will see the following message - 
<pre>
Untracked files:
      <strong>.gitignore</strong>
</pre>

We can see that <em>app.log</em> has already been ignored from the repository, but the <strong>.gitignore</strong> file is being tracked now. If we want the changes to take place properly, we need to commit the repository using <code>git commit -am "Adding .gitignore file"</code> in the git bash or terminal (Otherwise, first do <code>git add .</code> and then type in <code>git commit -m "Adding .gitignore file"</code>). When we check the status of the repository, we will see that we are back to a clean working directory.

We can check the files in our repository by listing the files in the terminal (Windows: <code>dir</code> & Linux/Mac: <code>ls -la</code>) and we can see that app.log is still in the repository, but it is not being tracked by git i.e., it is being ignored by git, because it is mentioned inside <strong>.gitignore</strong> file.

For now, we can simply go ahead and remove app.log entirely, from the terminal (Windows: <code>del app.log</code> & Linux/Mac: <code>rm app.log</code>).

[Goto: Table Of Contents](https://github.com/Ch-sriram/Just-Git-In#table-of-contents)

## 7. Advanced Version Control Using Git

In this section, we will learn more advanced concepts and techniques in git that apply in local repository. Some of the topics covered in this section include: the following topics:
- Comparing Differences,
- Branching, Merging & Conflict Resolution,
- Marking Milestones w. Tagging,
- How to save Work in Progress,
- How to Time Travel, Other, etc.

[Goto: Table Of Contents](https://github.com/Ch-sriram/Just-Git-In#table-of-contents)

### 7.1 Comparing Differences in Git

We will know how to compare differences using the <strong>diff</strong> and the <strong>difftool</strong> command in Git. The <code>difftool</code> command will only work if P4Merge is properly setup as the difftool, shown in [Git & GitHub Installations](https://github.com/Ch-sriram/Just-Git-In#5-git--github-installation) (section 5). 

In our demo repository, we are on the <em>master</em> branch with nothing to commit and with a clean working directory. When we type in our git command alias that we created earlier which is <code>git hist</code>, we will see all the commits that we made till now (i.e., the commit history of our repository this far). If we want to see the differences between two commit points, we can simply copy the hash-key (SHA1 Key) for the respective commit, and check it against the latest commit (which is the commit pointed by the HEAD pointer) using <code>git diff c904e33 HEAD</code> command in the terminal. We will get the difference between the HEAD's commit (which is the latest commit on the current (master) branch) and the respective commit that we mentioned earlier (which is c904e33 in our case).

<sup>Note: *Instead of "c904e33", we can use any SHA1 key which is actually a hash key associated to a commit.*</sup>

If we have the difftool configured as P4Merge, then we can type in almost the same command with a few changes as follows: <code>git difftool c904e33 HEAD</code>. We will have multiple files that are associated with the respective diff, therefore, to cycle through each one of them by quitting P4Merge with <code>Command + Q</code> (Windows: <code>Ctrl + Q</code>). After cycling through all the files in P4Merge difftool, git returns us back to the terminal.

Now, if we modify the LICENCE.md file, and we want to know the changes that we made to the repository compared to the HEAD's commit (i.e., latest commit), we simply type in <code>git diff</code> command in the terminal and we will see the latest uncommitted changes that are/were made to the repository's files.

In the same fashion as above, we can do the same thing, but instead, we will use the P4Merge difftool. For that, we type in <code>git difftool</code> command in the terminal. After we are done looking into the changes/modifications to the files in the git repository, we can quit the difftool (P4Merge) using <code>Command + Q</code> (Windows: <code>Ctrl + Q</code>).

To check all the options available with the <strong>diff</strong> command, we can always type in <code>git help diff</code> command in the terminal and get the manual page (documentation) on the <strong>diff</strong> command.

For the most part, anything that can be passed into the <strong>diff</strong> command, can also be passed into the <strong>difftool</strong> command (iff, difftool is configured properly).

[Goto: Table Of Contents](https://github.com/Ch-sriram/Just-Git-In#table-of-contents)

### 7.2 Branching and Merging Types in Git

Branching and Merging are very important concepts in Git.

<strong>Branch is just a timeline of Commits, more accurately, branches are the names/labels we give to timelines in Git</strong>. We can create/delete branches w/o affecting the timeline, all we are doing is creating/deleting labels of commits in Git. <strong>So far, we've been working on the default branch, which is the master branch</strong>. Now, we can create a new branch (say <strong>feature branch</strong>) to develop a new feature of our application in that new branch and then <strong>rejoin/merge</strong> that new branch to the master branch by merging in any changes that occurred on the new branch.

While Merging, Git tries it's best to automatically merge when possible, which leads to several types of merge scenarios. These types of merge scenarios are:
1. <strong>Fast-forward Merge</strong>: This merge happens in the simplest of cases when no additional work has been detected on the parent branch (by default, the master branch). Git will simply apply all commits from the other branch(s) directly onto the parent branch (as if we never branched off to begin with). We can manually disable the fast-forward merges if we don't desire them for some reason.
2. <strong>Automatic Merge</strong>: This happens when git detects non-conflicting changes in the parent branch. Git is able to automatically resolve any conflicts. In doing so, the old branch's timeline is preserved and a new merge commit is created to show the merging of the two branches. 
3. <strong>Manual Merge</strong>: This happens when git is unable to automatically resolve any conflicts. Git enters a special conflicting merge state, which means that all merge conflicts must be resolved prior to moving forward with a commit. Once all conflicts have been resolved, those changes are saved as a merge commit.

[Goto: Table Of Contents](https://github.com/Ch-sriram/Just-Git-In#table-of-contents)

### 7.3 Special Markers/Pointers

In addition branches, tags and other labels for commits, Git has special markers (or pointers). One such popular marker is called <strong>HEAD</strong> which points to the Last Commit of Current Branch, it means that, as we switch branches, the location of <strong>HEAD</strong> pointer moves to match the last commit location of that branch.

While <strong>HEAD</strong> automatically points to the last commit of the current branch, it is also possible to move the <strong>HEAD</strong> pointer manually to a commit we wish to move it to. The details on how to manually move the <strong>HEAD</strong> pointer to a commit of our choice, will be covered later.

For now, we just need to remember that <strong>HEAD</strong> points to the last commit of the current branch.

[Goto: Table Of Contents](https://github.com/Ch-sriram/Just-Git-In#table-of-contents)

### 7.4 Example of Branching

We will create and manage branches (other than master) in our git repository in this section. Currently we are in the demo repository where, if we check the status of the repository, we will see the following message:
<pre>
Changes not staged for commit:
      <strong>modified:    README.md</strong>
</pre>

Now assume that we intended that README.md file was to be modified experimentally as a feature that we are testing for our app for the next update. Either way, we can use feature/topic branches in order to separate out changes that we want to make off of the master branch. If we use the <code>git branch</code> command, we will see the following response in the terminal:
<pre>
* <strong>master</strong>
</pre>
which basically means that we are currently working on a single branch which is the <em>master</em> branch. Now, we can create another branch by using the <strong>branch</strong> command and then separately switch to that branch. But we can accomplish both actions (i.e., creating a new branch and switching to that new branch) by using the <strong>checkout</strong> command with <strong>-b</strong> option. Syntax: <code>git checkout -b branch-name</code>. Example usage: <code>git checkout -b updates</code>. Here, "updates" is the name of the new branch. When we type in the <strong>git checkout</strong> command, we will see the following response in the terminal:
<pre>
M     README.md
Switched to a new branch 'updates'
</pre>
Now here, a couple of things have happened. First, it created a new branch called 'updates'. Second, git automatically switched to that new branch. And, since there were modifications pending in the working directory (related to README.md), it carried those modifications forward, into that new branch "updates". This is a technique that we can use when we start working on the <em>master</em> branch, and we decide later that before committing, these changes should really be isolated into their own feature/topic branch.

Now we can modify the README.md file as we want and then add the changes to the staging area using <code>git add .</code> command. After that, we can simply commit the changes into the "updates" branch using <code>git commit -m "Adding new updates from master branch to 'updates' branch"</code> command, and we will see the following response in the terminal:
<pre>
[updates 9394c33] Adding new updates from master branch to 'updates' branch
1 file changed, 40 insertions(+), 5 deletions(-)
</pre>

When we type in <code>git status</code> in our repository now, we will see the following response in the terminal:
<pre>
On branch updates
nothing to commit, working directory clean
</pre>

Now when we type in our git alias i.e., <code>git hist</code>, we will see something similar to the following response in the terminal:
<pre>
* 9394c33 (<strong>HEAD -> updates</strong>) Adding new updates from master branch to 'updates' branch
* 6b79701 (<strong>master</strong>) README Update
* 20c7c63 Adding .gitignore file
* eb94f26 Adding .gitignore file
* 801a434 README Update
* cd82d85 README Updated
* 1f28d75 deleted demo.txt file
* 64f7486 renamed example.txt to demo.txt
* 53f8779 adding example.txt
* d741b7e README Update
* 6bf863a README Update
* 634793a README Update
* 8af524a README & LICENCE Update
* 231b4cd README Update
</pre>

We can see that the latest commit is on the "updates" branch and the previous commit is on "master" branch. We can see what the changes are using the <code>git diff updates master</code> command. Note that the <strong>diff</strong> command allows us to pass in the names of the branches instead of the commit ID's (which are the SHA1 Keys). The <strong>diff</strong> command above will show the differences in both the branches (mainly, the modifications made to the files in the repository w.r.t the branches).

In order to integrate any changes made in "updates" branch, we need to first switch to the parent branch, which is the "master" branch. To switch branches, we use the <strong>checkout</strong> command. Syntax: <code>git checkout branch-name</code>. Example usage: <code>git checkout master</code>. Now, we will look into the log/history from <em>master</em> branch's perspective by typing in <code>git hist</code> command in the terminal. We should get a response which is somewhat similar to the following:
<pre>
* 9394c33 (<strong>updates</strong>) Adding new updates from master branch to 'updates' branch
* 6b79701 (<strong>HEAD -> master</strong>) README Update
* 20c7c63 Adding .gitignore file
* eb94f26 Adding .gitignore file
* 801a434 README Update
* cd82d85 README Updated
* 1f28d75 deleted demo.txt file
* 64f7486 renamed example.txt to demo.txt
* 53f8779 adding example.txt
* d741b7e README Update
* 6bf863a README Update
* 634793a README Update
* 8af524a README & LICENCE Update
* 231b4cd README Update
</pre>

We can see that <strong>HEAD</strong> is pointing to the <em>master</em> branch, and HEAD typically points to the last commit on the current branch, and therefore, the current branch is <em>master</em> and the last commit on the current branch is the top one in the log as shown above, and therefore, HEAD and master are sharing the same commit ID. 

Now we can go ahead and merge in the changes made in the <em>updates</em> branch into the <em>master</em> branch using <code>git merge updates</code> command in the terminal. Note that <strong>HEAD</strong> is currently pointing the <em>master</em> branch's latest commit and therefore, in <code>git merge branch-name</code>, we wrote "updates" for the "branch-name".

Now, after we merge, we would see a message that should be somewhat similar to the following:
<pre>
Updating 6b79701...9394c33
Fast-forward
 README.md | 45 ++++--
 1 file changed, 40 insertions(+), 5 deletions(-)
</pre>

This merge that we did just now, was the most simple merge, where we simply did a fast forward type merge, which means that we are going to pretend that we never really switched away from the <em>master</em> branch and we merge the changes from the <em>updates</em> branch into the <em>master</em> branch. Therefore, we are going to apply these commits directly to the master branch.

Now, if we type in <code>git hist</code> (our git alias) command, we should see some message that looks as follows:
<pre>
* 9394c33 (<strong>HEAD -> master, updates</strong>) Adding new updates from master branch to 'updates' branch
* 6b79701 README Update
* 20c7c63 Adding .gitignore file
* eb94f26 Adding .gitignore file
* 801a434 README Update
* cd82d85 README Updated
* 1f28d75 deleted demo.txt file
* 64f7486 renamed example.txt to demo.txt
* 53f8779 adding example.txt
* d741b7e README Update
* 6bf863a README Update
* 634793a README Update
* 8af524a README & LICENCE Update
* 231b4cd README Update
</pre>

We can see that <strong>HEAD</strong>, <em>master</em> and <em>updates</em> branch's pointers, all point to the same commit ID (which is 9394c33 in this case) and that's the affect of a fast-forward merge. There are options to disable the fast-forward merges from happening, but most of the time, we'll want this behaviour to be intact.

Once we have completed merging in our changes from the <em>updates</em> branch to the <em>master</em> branch, we no longer need the <em>updates</em> branch to be present in our git repository, because effectively, branches in Git are just labels of timelines, and once they've been integrated into the main timeline, there's no need for them anymore. Therefore, we delete the branch(s) that we do not need anymore using <code>git branch -d updates</code> command in the terminal, where <em>updates</em> is the branch-name we want to delete. We should get some message similar to the following: 
<pre>
Deleted branch updates (was 9394c33)
</pre>

Again, when we type in <code>git branch</code>, we will see the following response:
<pre>
* <strong>master</strong>
</pre>

Now, if we use our git log alias which is <code>git hist</code>, we will be seeing something of the following sort:
<pre>
* 9394c33 (<strong>HEAD -> master</strong>) Adding new updates from master branch to 'updates' branch
* 6b79701 README Update
* 20c7c63 Adding .gitignore file
* eb94f26 Adding .gitignore file
* 801a434 README Update
* cd82d85 README Updated
* 1f28d75 deleted demo.txt file
* 64f7486 renamed example.txt to demo.txt
* 53f8779 adding example.txt
* d741b7e README Update
* 6bf863a README Update
* 634793a README Update
* 8af524a README & LICENCE Update
* 231b4cd README Update
</pre>

We can see that we no longer have the <em>updates</em> branch associated with the respective commit ID (in our case, it is 9394c33). Also note that the actual log/history did NOT vanish/go-away, just the label i.e., <em>updates</em> was removed.

[Goto: Table Of Contents](https://github.com/Ch-sriram/Just-Git-In#table-of-contents)

### 7.5 Conflict Resolution While Merging

This time, we will deliberately cause a conflict in our git repository and then resolve that conflict when working with branches. We will cause a conflict in the LICENCE.md file. 

We are currently in the demo git repository from where, if we check the status of our git repository (using <code>git status</code>), we will see that we are on branch <em>master</em> and the working directory is clean with nothing to commit.

From the <em>master</em> branch, we will open the LICENCE.md file and then make changes to it. We will add the 3<sup>rd</sup> line with the string "This is some change!!" as seen below:

<strong>LICENCE.md</strong>
<pre>
# LICENCE
## [Licence Name] - [Some Text], just for this tutorial.
This is some change!!
</pre>

We will save and get back to the terminal and then create a branch, say <strong>very-bad</strong> branch using <code>git checkout -b very-bad</code> command in the terminal. We should see the following message as a response from the terminal:
<pre>
Switched to a new branch 'very-bad'
</pre>

Now if we type in <code>git branch -a</code> in the terminal, we should a response that is somewhat similar to the following message:
<pre>
  master
* <strong>very-bad</strong>
</pre>

which means that we are currently working with the <em>very-bad</em> branch (or timeline).

Now we will modify our LICENCE.md file such that it will cause a conflict. To do that, we have to update the same part of the file on both the branches (viz. <em>master</em> and <em>very-bad</em>). Therefore, we will update the 3<sup>rd</sup> line of LICENCE.md file with the string "This is bound to cause trouble!" as seen below:

<strong>LICENCE.md</strong>
<pre>
# LICENCE
## [Licence Name] - [Some Text], just for this tutorial.
This is bound to cause trouble!
</pre>

We will save and close that change and then commit using <code>git commit -am "very bad update in LICENCE.md"</code> command in the terminal. We should see something of the following sort in our terminal:
<pre>
[very-bad 809b141] very bad update in LICENCE.md
 1 file changed, 1 insertion(+), 1 deletion(-)
</pre>

When we use our pre-defined git alias for the log, which is <code>git hist</code>, we should something of the similar sort in our terminal:
<pre>
* 809b141 (<strong>HEAD -> very-bad</strong>)
* 9394c33 (<strong>master</strong>) Adding new updates from master branch to 'updates' branch
* 6b79701 README Update
* 20c7c63 Adding .gitignore file
* eb94f26 Adding .gitignore file
* 801a434 README Update
* cd82d85 README Updated
* 1f28d75 deleted demo.txt file
* 64f7486 renamed example.txt to demo.txt
* 53f8779 adding example.txt
* d741b7e README Update
* 6bf863a README Update
* 634793a README Update
* 8af524a README & LICENCE Update
* 231b4cd README Update
</pre>

Now, we will switch to <em>master</em> branch using <code>git checkout master</code> command in the terminal. We should see the following message in the terminal:
<pre>
Switched to branch 'master'
</pre>

Before we merge in the changes, we are going to think about this scenario as us being another developer who didn't know about the changes made to the LICENCE.md file at the 3<sup>rd</sup> line, and therefore, we will make another change at the 3<sup>rd</sup> line of the LICENCE.md file with the string "I hope this is not much of a problem!!!". The changes made should look as the file shown below:

<strong>LICENCE.md</strong>
<pre>
# LICENCE
## [Licence Name] - [Some Text], just for this tutorial.
I hope this is not much of a problem!!!
</pre>

Save and close the LICENCE.md file and in the terminal, we will again do the express commit using <code>git commit -am "LICENCE.md Update (Merge Conflict Possible)"</code>. Now we will merge the <em>very-bad</em> branch into the <em>master</em> branch using <code>git merge very-bad</code> command in the terminal, and we should see a message of the following sort:
<pre>
Auto-merging LICENCE.md
CONFLICT (content): Merge conflict in LICENCE.md
Automatic merge failed; fix conflicts and then commit the result.
</pre>

Therefore as we can see, due to the multiple changes of the same file at the same location of the two branches, the auto-merge functionality, when merging the branches, doesn't know which version of the LICENCE.md to keep in the repository. Therefore, there's a conflict here, which places us in a <strong>MERGING state</strong> which is denoted by our git bash as the following:
<pre>
(master|MERGING) demo $ 
</pre>

Now, when we see the contents of the LICENCE.md file (because LICENCE.md file is the file that's implicated in the merge conflict) using <code>cat LICENCE.md</code> in git bash, we should the contents of the file somewhat similar to the following:

<strong>LICENCE.md</strong>
<pre>
# LICENCE
## [Licence Name] - [Some Text], just for this tutorial.
&lt;&lt;&lt;&lt;&lt;&lt;&lt;&lt; HEAD
I hope this is not much of a problem!!!
========
This is bound to case trouble!
&gt;&gt;&gt;&gt;&gt;&gt;&gt;&gt; very-bad
</pre>

Now, the current version of the file has these weird caret symbol(s) [< and >] which denote the part(s) of the file that is/are conflicted. We can see that the conflict is between the content of either <strong>HEAD</strong> (which is master in this case) or <strong>very-bad</strong> and since this happens to be a very simple case of the merge conflict, we could manually modify the LICENCE.md file using our merge tool (which is P4Merge Helix) that we configured earlier in section 5 ([Git & GitHub Installation]()).

Therefore, we use the merge tool using <code>git mergetool</code> while in the MERGING state and we will see that P4Merge launches with a 3-way merge in progress. We can select any one of the 3 versions of LICENCE.md file and then save that version. Once we've done that, we have no further conflicts to resolve and therefore, we can quit P4Merge altogether. To complete the merge, we need to commit what we've saved and so, we type in <code>git commit -m "Resolving Conflict in LICENCE.md"</code> in the git bash. If the message in response is the following:
<pre>
[master a78ed77] Resolving Conflict in LICENCE.md
</pre>

then the merge conflict has definitely been resolved and we will return back to the git bash in the normal state from the MERGING state, which will look as follows:
<pre>
(master) demo $
</pre>

We check the status of our repository using <code>git status</code> and we can see the following message in our terminal:
<pre>
Untracked files:
      <strong>LICENCE.md.orig</strong>
</pre>

We can see that we have a <strong>LICENCE.md.orig</strong> file which is untracked. A file with <strong>.orig</strong> extension means that it is the original version of the that respective file. Now, we don't need the <em>.orig</em> files to be tracked by our git repository, and therefore, we can add all <strong>.orig</strong> files to be excluded from our repository in the <strong>.gitignore</strong> file as follows:

<strong>.gitignore</strong>
<pre>
*.log
*.orig
</pre>

When we check the status of our repository, we will see the following message:
<pre>
On branch master
Changes not staged for commit:
      <strong>modified:    .gitignore</strong>
</pre>

We will express commit the current state of our repository using <code>git commit -am "Updating .gitignore to exclude .orig files"</code> command in our terminal and we should see the following response in the terminal:
<pre>
[master df3d921] Updating .gitignore to exclude .orig files
 1 file changed, 2 insertions(+), 1 deletion(-)
</pre>

Now, all the files with <strong>.orig</strong> extension will be excluded from being tracked in our git repository and therefore, we can go ahead and delete LICENCE.md.orig (Windows: <code>del LICENCE.md.orig</code> & Linux/Mac: <code>rm LICENCE.md.orig</code>).

[Goto: Table Of Contents](https://github.com/Ch-sriram/Just-Git-In#table-of-contents)

### 7.6 Marking Special Events w. Tagging

We are currently in the demo repository on the master branch. If we use our alias i.e., <code>git hist</code>, we should get something similar to the following response in the terminal:

<pre>
* 3c5ec7d (<strong>HEAD -> master</strong>) Updating .gitignore to exclude .orig files
*   afb7058 Resolving Conflict in LICENCE.md
|\
| * 7c48e4c (<strong>very-bad</strong>) very bad update in LICENCE.md
* | cb652a3 LICENCE.md Update (Merge Conflict Possible)
|/
* 85a1d27 README Update
* 593fe03 Adding new updates from master branch to 'updates' branch
* 6b79701 README Update
* 20c7c63 Adding .gitignore file
* eb94f26 Adding .gitignore file
* 801a434 README Update
* cd82d85 README Updated
* 1f28d75 deleted demo.txt file
* 64f7486 renamed example.txt to demo.txt
* 53f8779 adding example.txt
* d741b7e README Update
* 6bf863a README Update
* 634793a README Update
* 8af524a README & LICENCE Update
* 231b4cd README Update
</pre>

At this point, we have been working with our demo repository for a really long time. So, we can mark this point in the repository with some type of a milestone. To do that, Git supports a notion of <strong>tags</strong>, which are just labels that we can put at any arbitrary commit point. By default, if we don't specify a commit (i.e., commit ID), it will be the current commit or <strong>HEAD</strong>. Now, there are two type of tags and they're:

1. <strong>Lightweight Tags</strong>: It is simply a tag which just has a name associated to it. We create a lightweight tag using the <code>git tag tag-name</code> command (ex: <code>git tag mytag</code>). Now, if we type in <code>git tag --list</code>, we will see the following response in the terminal:

<pre>
mytag
</pre>

which is essentially a list of tags we have made. And, if we check all the logs using our alias that we created i.e., <code>git hist</code>, we should something similar to the following response in the terminal:

<pre>
* 3c5ec7d (<strong>HEAD -> master, tag: mytag</strong>) Updating .gitignore to exclude .orig files
*   afb7058 Resolving Conflict in LICENCE.md
|\
| * 7c48e4c (<strong>very-bad</strong>) very bad update in LICENCE.md
* | cb652a3 LICENCE.md Update (Merge Conflict Possible)
|/
* 85a1d27 README Update
* 593fe03 Adding new updates from master branch to 'updates' branch
* 6b79701 README Update
* 20c7c63 Adding .gitignore file
* eb94f26 Adding .gitignore file
* 801a434 README Update
* cd82d85 README Updated
* 1f28d75 deleted demo.txt file
* 64f7486 renamed example.txt to demo.txt
* 53f8779 adding example.txt
* d741b7e README Update
* 6bf863a README Update
* 634793a README Update
* 8af524a README & LICENCE Update
* 231b4cd README Update
</pre>

Now, this is a lightweight tag and so there's no associated information with it.

2. <strong>Annotated Tags</strong>: These tags should be preferred over lightweight tags when we have several releases of the app we are working on, and also, each release/version of the app has some changelog associated with itself. Annotated tags have extra information associated with the tag. Before we create an annotated tag, we will delete the lightweight tag we created earlier (i.e., mytag) using <code>git tag -d tag-name</code> (ex: <code>git tag -d mytag</code>) command in the terminal and we should see the following response in the output:

<pre>
Deleted tag 'mytag' (was 3c5ec7d)
</pre>

Now, to create an annotated tag, we use the command syntax as <code>git tag -a tag-name -m "commit-message"</code> (ex: <code>git tag -a v1.0 -m "Release 1.0"</code>) in the terminal. We will see the list of tags we have using <code>git tag --list</code> command in the terminal, and we should get the following output:

<pre>
v1.0
</pre>

When we type in <code>git hist</code>, we will see the following output in the terminal:

<pre>
* 3c5ec7d (<strong>HEAD -> master, tag: v1.0</strong>) Updating .gitignore to exclude .orig files
*   afb7058 Resolving Conflict in LICENCE.md
|\
| * 7c48e4c (<strong>very-bad</strong>) very bad update in LICENCE.md
* | cb652a3 LICENCE.md Update (Merge Conflict Possible)
|/
* 85a1d27 README Update
* 593fe03 Adding new updates from master branch to 'updates' branch
* 6b79701 README Update
* 20c7c63 Adding .gitignore file
* eb94f26 Adding .gitignore file
* 801a434 README Update
* cd82d85 README Updated
* 1f28d75 deleted demo.txt file
* 64f7486 renamed example.txt to demo.txt
* 53f8779 adding example.txt
* d741b7e README Update
* 6bf863a README Update
* 634793a README Update
* 8af524a README & LICENCE Update
* 231b4cd README Update
</pre>

So far, we haven't seen any difference between a lightweight tag and an annotated tag. The question remains, where does the annotation (i.e., the commit message that we typed in) come in? To view the annotations of an annotated tag, we type in <code>git show tag-name</code> (ex: <code>git show v1.0</code>), we should see something similar to the following output in the terminal:

<pre>
tag v1.0
Tagger: Chandrabhatta Sriram &lt;sriram@example.com>
Date:   Sun Mar 15 19:23:33 2020 +0530

Release 1.0

commit 3c5ec7d224122896467386d56b6b12dd6336698c (HEAD -> master, tag: v1.0)
Author: Chandrabhatta Sriram &lt;sriram@example.com>
Date:   Sun Mar 15 12:24:56 2020 +0530

    Updating .gitignore to exclude .orig files

diff --git a/.gitignore b/.gitignore
index bf0824e..490a1a0 100644
--- a/.gitignore
+++ b/.gitignore
@@ -1 +1,2 @@
-*.log
\ No newline at end of file
+*.log
+*.orig
\ No newline at end of file
</pre>

We can see that it has the information about the Tagger, Date that the respective version of the repository was tagged, the commit message (in this case "Release 1.0") followed by the rest of the information for the commit that's associated with that tag. These annotated tags are really useful when we are trying to note major milestones/versions/releases of our repository, and we generally, might want to associate some information with those major releases/versions and that could be achieved through tagging.

[Goto: Table Of Contents](https://github.com/Ch-sriram/Just-Git-In#table-of-contents)

### 7.7 Saving Work in Progress w. Stashing

We are currently in the demo repository on the master branch in a clean working directory. We will modify the README.md file and we check the status of our repository using <code>git status</code> and we should see the following output:

<pre>
On branch master
Changes not staged for commit:
      <strong>modified:    README.md</strong>
</pre>

But, what if decide we are really supposed to be working on something other than the README.md file. Therefore, what we can do is, we can stash the changes made in README.md using <code>git stash</code> command in the terminal and we should see something similar to the following output:

<pre>
Saved working directory and index state WIP on master: 057fdf2 README Update
</pre>

We can now check the status of the repository using <code>git status</code>, we will see the following output in the terminal:

<pre>
On branch master
nothing to commit, working tree clean
</pre>

Now, if we type in <code>git stash list</code>, it will show us the list of things we stashed, i.e., the following output in the terminal:

<pre>
stash@{0}: WIP on master: 057fdf2 README Update
</pre>

Now, we stashed the previous modification, therefore, we can make changes to something other than the README.md file. Let's say we make changes to the LICENCE.md file and apply those changes using git's express commits i.e., <code>git commit -am "Updating LICENCE.md"</code> and we should some output similar to the following in the terminal:

<pre>
[master 2bbc636] Updating LICENCE.md
 1 file changed, 1 insertion(+), 1 deletion(-)
</pre>

When we check the status of our repository using <code>git status</code>, we should see the following output:

<pre>
On branch master
nothing to commit, working tree clean
</pre>

Now, from the stash, we will apply our stash using <code>git stash pop</code> command, which will do 2 actions at once which are the same as <code>git stash apply</code> and then <code>git stash drop</code> at the same time, which translates to apply the last stash in the stash stack (for <code>git stash apply</code> [In this case, we put the changes that we made in the README.md file, back into the README.md file]) and drop/delete that stash from the top of the stash stack, which was just applied (for <code>git stash drop</code> [In this case, it will drop/delete the stash@{0} which was the stash for the Commit ID 057fdf2 "README Update"]). After <code>git stash pop</code>, we should see the following output in the terminal:

<pre>
On branch master
Changes not staged for commit:
      <strong>modified:    README.md</strong>
</pre>

Now if we type in <code>git stash list</code> we would get no result in the terminal. And if we check the README.md file, we can see that README.md file was updated like it was updated before the stash ever took place. Now we can commit the README.md's update using express commit i.e., using <code>git commit -am "README update after stash"</code> command in the terminal and we should something similar to the following output:

<pre>
[master 78c2353] README update after stash
 1 file changed, 1 insertion(+), 1 deletion(-)
</pre>

When we check the status of our repository using <code>git status</code> command in the terminal, we should see the following output:

<pre>
On branch master
nothing to commit, working tree clean
</pre>

[Goto: Table Of Contents](https://github.com/Ch-sriram/Just-Git-In#table-of-contents)

### 7.8 Time Travel w. Reset & Reflog

We are currently in the demo repository, on the master branch and the working directory is clean.

We will update our README.md file and then add the changes to the staging area, and so when we see the status of our git repository using <code>git status</code>, we should see a response in the terminal that's somewhat similar to the following:

<pre>
On branch master
Changes to be committed:
      <strong>modified:    README.md</strong>
</pre>

We again, add some new content into README.md and check the status again. This time, we should see the following output in the terminal:

<pre>
On branch master:
Changes to be committed:
      <strong>modified:    README.md</strong>

Changes not staged for commit:
      <strong>modified:    README.md</strong>
</pre>

We can see that we've our modifications detected in both the staging area and in our working directory.

Now, there maybe times when we need to go to a different commit point. Example: If we made a mistake in the last commit that we shouldn't have committed in the first place, then we would want to rollback to a previous commit before that last commit. To check all the commits we ever made, we will use our git alias i.e, using <code>git hist</code> (which is same as <code>git log --all --oneline --graph --decorate</code>) command and we should see something similar to the following output in our terminal:

<pre>
* 184db4d (<strong>HEAD -> master</strong>) README.md updated after it was stashed
* 445064a LICENCE.md updated when README.md's update was stashed
* 057fdf2 README Update
* 3c5ec7d (<strong>tag: v1.0</strong>) Updating .gitignore to exclude .orig files
*   afb7058 Resolving Conflict in LICENCE.md
|\
| * 7c48e4c (<strong>very-bad</strong>) very bad update in LICENCE.md
* | cb652a3 LICENCE.md Update (Merge Conflict Possible)
|/
* 85a1d27 README Update
* 593fe03 Adding new updates from master branch to 'updates' branch
* 6b79701 README Update
* 20c7c63 Adding .gitignore file
* eb94f26 Adding .gitignore file
* 801a434 README Update
* cd82d85 README Updated
* 1f28d75 deleted demo.txt file
* 64f7486 renamed example.txt to demo.txt
* 53f8779 adding example.txt
* d741b7e README Update
* 6bf863a README Update
* 634793a README Update
* 8af524a README & LICENCE Update
* 231b4cd README Update
</pre>

We can see that we've several commits to choose from. So we can select a commit point (or version of our app) and <strong>reset</strong> our git repository to that commit point. For that, we use <code>git reset commit-ID --reset-type</code> command (ex: <code>git reset 3c5ec7d --soft</code>). For the --reset-type, we actually have 3 distinct ways of resetting:

1. <strong>Soft Reset</strong>: This is the least destructive out of all the rest type we have. It means that, soft reset only changes where the <strong>HEAD</strong> pointer points to, to the commit point we specified. Now, if we see where <strong>HEAD</strong> is pointing to, we can see that it is pointing to 184db4d (which is the master branch for now). Now, if we type in <code>git reset 3c5ec7d --soft</code> and then we type in <code>git hist</code>, we should see something similar to the following output in the terminal:

<pre>
* 3c5ec7d (<strong>HEAD -> master, tag: v1.0</strong>) Updating .gitignore to exclude .orig files
*   afb7058 Resolving Conflict in LICENCE.md
|\
| * 7c48e4c (<strong>very-bad</strong>) very bad update in LICENCE.md
* | cb652a3 LICENCE.md Update (Merge Conflict Possible)
|/
* 85a1d27 README Update
* 593fe03 Adding new updates from master branch to 'updates' branch
* 6b79701 README Update
* 20c7c63 Adding .gitignore file
* eb94f26 Adding .gitignore file
* 801a434 README Update
* cd82d85 README Updated
* 1f28d75 deleted demo.txt file
* 64f7486 renamed example.txt to demo.txt
* 53f8779 adding example.txt
* d741b7e README Update
* 6bf863a README Update
* 634793a README Update
* 8af524a README & LICENCE Update
* 231b4cd README Update
</pre>

Now we can see that the <strong>HEAD</strong> is pointing to 3c5ec7d which is commit ID that we passed in earlier to the <strong>reset</strong> command. If we check our repository's status using <code>git status</code>, we can see something similar to the following output in the terminal:

<pre>
On branch master
Changes to be committed:
      <strong>modified:    LICENCE.md</strong>
      <strong>modified:    README.md</strong>

Changes not staged for commit:
      <strong>modified:    README.md</strong>
</pre>

We can see that we have files that are modified in the working directory and in our staging area and this is what the <strong>Soft Reset</strong> precisely allows us to do and it is simply changing the Commit ID that the <strong>HEAD</strong> pointer is pointing to, to the respective Commit ID we pass in as the parameter when we use the <strong>reset</strong> command. Therefore a soft reset preserves the Git staging area and our working directory, which effectively means that, we can back out our changes, make minor modifications to them, and then commit where <strong>HEAD</strong> is currently pointing to.

2. <strong>Mixed/Default Reset</strong>: Let's say we will reset to the Commit ID - 20c7c63 ("Adding .gitignore file") using <code>git reset 20c7c63 --mixed</code> (Note that by default, <code>git reset 20c7c63 --mixed</code> means the same as <code>git reset 20c7c63</code>. It means that if no option is given to the <strong>reset</strong> command, by default, --mixed option is applied) command in the terminal, and instantly, we would some message of the following sort:

<pre>
Unstaged changes after reset:
M     .gitignore
M     LICENCE.md
M     README.md
</pre> 

We can see that some of the changes made till now have been unstaged. If we use our log alias i.e., <code>git hist</code>, we should some output of the following sort:

<pre>
* 3c5ec7d (<strong>tag: v1.0</strong>) Updating .gitignore to exclude .orig files
*   afb7058 Resolving Conflict in LICENCE.md
|\
| * 7c48e4c (<strong>very-bad</strong>) very bad update in LICENCE.md
* | cb652a3 LICENCE.md Update (Merge Conflict Possible)
|/
* 85a1d27 README Update
* 593fe03 Adding new updates from master branch to 'updates' branch
* 6b79701 README Update
* 20c7c63 (<strong>HEAD -> master</strong>) Adding .gitignore file
* eb94f26 Adding .gitignore file
* 801a434 README Update
* cd82d85 README Updated
* 1f28d75 deleted demo.txt file
* 64f7486 renamed example.txt to demo.txt
* 53f8779 adding example.txt
* d741b7e README Update
* 6bf863a README Update
* 634793a README Update
* 8af524a README & LICENCE Update
* 231b4cd README Update
</pre>

We can see that the <strong>HEAD</strong> is pointing to 20c7c63. And if we check the status using <code>git status</code> command, we should some output which is similar to the following:

<pre>
On branch master
Changes not staged for commit:
      <strong>modified:   .gitignore</strong>
      <strong>modified:   LICENCE.md</strong>
      <strong>modified:   README.md</strong>
</pre>

We can see that we have several files that have been unstaged and have been placed into our working directory; there's nothing in our staging area.

3. <strong>Hard Reset</strong>: This type of reset is the most destructive of all the reset modes. To apply this reset, we will simply apply the <strong>reset</strong> command to a particular Commit ID using the --hard option i.e., using the <code>git reset commit-id reset-type</code> command (ex: <code>git reset 8af524a --hard</code>) and we should get an output that's similar to the following:

<pre>
HEAD is now at 8af524a README & LICENCE Update
</pre>

If we now check the status of our repository using <code>git status</code>, we will see the following message:

<pre>
On branch master
nothing to commit, working directory clean
</pre>

By the output above, we can see that any changes that were pending till now, have been wiped out (along with anything that was in the staging area) when we did a hard reset. Apart from a handful of changes we have made at the very beginning, we really haven't lost a whole lot. Now, if we type in <code>git hist</code>, we will see the following output:

<pre>
* 3c5ec7d (<strong>tag: v1.0</strong>) Updating .gitignore to exclude .orig files
*   afb7058 Resolving Conflict in LICENCE.md
|\
| * 7c48e4c (<strong>very-bad</strong>) very bad update in LICENCE.md
* | cb652a3 LICENCE.md Update (Merge Conflict Possible)
|/
* 85a1d27 README Update
* 593fe03 Adding new updates from master branch to 'updates' branch
* 6b79701 README Update
* 20c7c63 Adding .gitignore file
* eb94f26 Adding .gitignore file
* 801a434 README Update
* cd82d85 README Updated
* 1f28d75 deleted demo.txt file
* 64f7486 renamed example.txt to demo.txt
* 53f8779 adding example.txt
* d741b7e README Update
* 6bf863a README Update
* 634793a README Update
* 8af524a (<strong>HEAD -> master</strong>) README & LICENCE Update
* 231b4cd README Update
</pre>

We can see that our <strong>HEAD</strong> is now pointing to the Commit ID - 8af524a ("README & LICENCE Update"). If we just type in <code>git log --oneline</code> command, we will see the following output in the terminal:

<pre>
8af524a README & LICENCE Update
231b4cd README Update
</pre>

We can see that we are not able to get all the commits we have made so far and that's because we did a hard reset. To check all the commits we've made so far, we use <code>git log --all</code> command. We can also use another command in conjunction with <strong>reset</strong> command, which is <code>git reflog</code>. Using <strong>reflog</strong> command is different when compared to <strong>log</strong> in the sense that <code>git log</code> shows us our commit IDs along with the timeline of our commits whereas <code>git reflog</code> shows us all the different actions we've taken while in the respective repository which will allow us to get all the way back to a specific commit ID, if we need to. The output in the terminal we get should resemble somewhat to the following (when we type in <code>git reflog</code>):

<pre>
8af524a HEAD@{0}: reset: moving to 8af524a
20c7c63 HEAD@{1}: reset: moving to 20c7c63
3c5ec7d HEAD@{2}: reset: moving to 3c5ec7d
184db4d (HEAD -> master) HEAD@{3}: commit: README.md updated after it was stashed
445064a HEAD@{4}: commit: LICENCE.md updated when README.md's update was stashed
057fdf2 HEAD@{5}: reset: moving to HEAD
057fdf2 HEAD@{6}: reset: moving to HEAD
057fdf2 HEAD@{7}: reset: moving to HEAD
057fdf2 HEAD@{8}: commit: README Update
3c5ec7d (tag: v1.0) HEAD@{9}: commit: Updating .gitignore to exclude .orig files
afb7058 HEAD@{10}: commit (merge): Resolving Conflict in LICENCE.md
cb652a3 HEAD@{11}: commit: LICENCE.md Update (Merge Conflict Possible)
85a1d27 HEAD@{12}: checkout: moving from very-bad to master
7c48e4c (very-bad) HEAD@{13}: commit: very bad update in LICENCE.md
85a1d27 HEAD@{14}: checkout: moving from master to very-bad
85a1d27 HEAD@{15}: commit: README Update
593fe03 HEAD@{16}: merge updates: Fast-forward
6b79701 HEAD@{17}: checkout: moving from updates to master
593fe03 HEAD@{18}: checkout: moving from master to updates
6b79701 HEAD@{19}: checkout: moving from updates to master
593fe03 HEAD@{20}: commit: Adding new updates from master branch to 'updates' branch
6b79701 HEAD@{21}: checkout: moving from master to updates
6b79701 HEAD@{22}: commit: README Update
20c7c63 HEAD@{23}: commit: Adding .gitignore file
eb94f26 HEAD@{24}: commit: Adding .gitignore file
801a434 HEAD@{25}: commit: README Update
cd82d85 HEAD@{26}: commit: README Updated
1f28d75 HEAD@{27}: commit: deleted demo.txt file
64f7486 HEAD@{28}: commit: renamed example.txt to demo.txt
53f8779 HEAD@{29}: commit: adding example.txt
d741b7e HEAD@{30}: commit: README Update
6bf863a HEAD@{31}: commit: README Update
634793a HEAD@{32}: commit: README Update
8af524a HEAD@{33}: commit: README & LICENCE Update
231b4cd HEAD@{34}: commit (initial): README Update
</pre>

Now, if we need to reset to HEAD@{3}, we can simply type in the commit ID associated with HEAD@{3} along with the reset command and the reset type. Now we are going to HEAD@{3} because HEAD@{3} is the last commit before we did any of the resets. Therefore, we type in <code>git reset 184db4d --hard</code> in the terminal and we should see the following output in the terminal:

<pre>
HEAD is now at 184db4d README.md updated after it was stashed
</pre>

We've now moved our Commit ID back to where it was in the beginning and therefore, we will type in <code>git log --oneline</code> and we should get the following output in the terminal:

<pre>
184db4d (HEAD -> master) README.md updated after it was stashed
445064a LICENCE.md updated when README.md's update was stashed
057fdf2 README Update
3c5ec7d (tag: v1.0) Updating .gitignore to exclude .orig files
afb7058 Resolving Conflict in LICENCE.md
cb652a3 LICENCE.md Update (Merge Conflict Possible)
7c48e4c (very-bad) very bad update in LICENCE.md
85a1d27 README Update
593fe03 Adding new updates from master branch to 'updates' branch
6b79701 README Update
20c7c63 Adding .gitignore file
eb94f26 Adding .gitignore file
801a434 README Update
cd82d85 README Updated
1f28d75 deleted demo.txt file
64f7486 renamed example.txt to demo.txt
53f8779 adding example.txt
d741b7e README Update
6bf863a README Update
634793a README Update
8af524a README & LICENCE Update
231b4cd README Update
</pre>

It looks like we have all our commits that we made till now, back again to us. Now if we use our <code>git hist</code> alias command, we should see the output as the following (which will look the same as applying <code>git hist</code> prior to applying any resets to the repository):

<pre>
* 184db4d (HEAD -> master) README.md updated after it was stashed
* 445064a LICENCE.md updated when README.md's update was stashed
* 057fdf2 README Update
* 3c5ec7d (tag: v1.0) Updating .gitignore to exclude .orig files
*   afb7058 Resolving Conflict in LICENCE.md
|\
| * 7c48e4c (very-bad) very bad update in LICENCE.md
* | cb652a3 LICENCE.md Update (Merge Conflict Possible)
|/
* 85a1d27 README Update
* 593fe03 Adding new updates from master branch to 'updates' branch
* 6b79701 README Update
* 20c7c63 Adding .gitignore file
* eb94f26 Adding .gitignore file
* 801a434 README Update
* cd82d85 README Updated
* 1f28d75 deleted demo.txt file
* 64f7486 renamed example.txt to demo.txt
* 53f8779 adding example.txt
* d741b7e README Update
* 6bf863a README Update
* 634793a README Update
* 8af524a README & LICENCE Update
* 231b4cd README Update
</pre>

[Goto: Table Of Contents](https://github.com/Ch-sriram/Just-Git-In#table-of-contents)

## 8. Basics of GitHub

GitHub is a git repository hosting service where we can host unlimited public/private repositories. In GitHub, we can create an account [here](https://github.com/join?source=header-home) and sign-in after creating an account [here](https://github.com/login).

After creating a GitHub account, we are all set to push our changes we made in our repository till now onto our Git Repository. We can create a repository in GitHub by following the steps provided [here](https://help.github.com/en/enterprise/2.13/user/articles/creating-a-new-repository).

[Goto: Table Of Contents](https://github.com/Ch-sriram/Just-Git-In#table-of-contents)

### 8.1 Linking to our GitHub Repository (Local <-> Remote)

In our demo repository our status is that  there nothing to commit and the working directory is clean on the master branch.

To connect our local repository to the remote repository (which is hosted by GitHub), we us the <strong>remote</strong> command. If we issue the <code>git remote -v</code> command, git responds without any result, that means that there's no remote repository connected to the respective local repository.

To connect to a remote repository, we first create a repository after following the steps present [here](https://help.github.com/en/enterprise/2.13/user/articles/creating-a-new-repository). We can link the local repository to our remote repository using the <strong>add</strong> sub-command in the <strong>remote</strong> command, i.e., using the syntax <code>git remote add origin https://github.com/username/repo-name.git</code> (Ex: <code>git remote add origin https://github.com/Ch-sriram/Just-Git-In.git</code>) where the <strong>add</strong> sub-command takes in <strong>two parameters</strong> which is the <strong>name of the remote reference we want to create (in this case it is 'origin')</strong> and the second parameter which is <strong>full URL to the remote repository</strong>. In this case we can refer to our remote repository with any name in place of 'origin', but by convention, the first and primary remote repository is named and refered by the name 'origin'. Now if we type in <code>git remote -v</code>, git responds with the following message in the terminal:

<pre>
origin https://github.com/Ch-sriram/Just-Git-In.git (fetch)
origin https://github.com/Ch-sriram/Just-Git-In.git (push)
</pre>

Git tells us that we've our origin point towards the remote git repository we mentioned earlier. Now there might be a confusion about why the remote repository's entry (URL) is listed twice (<strong>one for fetch</strong> and <strong>one for push</strong>)? That's because technically, git will allow to have two different URLs one for fetching the changes from the remote repository to the local repository and one for pushing the changes made in the local repository to the remote repository. The URL for fetching can be different compared to the URL for pushing the repository, but in most cases, the URLs for fetching and pushing will be the same.

[Goto: Table Of Contents](https://github.com/Ch-sriram/Just-Git-In#table-of-contents)

### 8.2 Pushing Changes to GitHub (Local to Remote)

We are currently in demo git repository in a clean working directory on master branch with nothing to commit.

Now that we have connected our local repository with the remote repository, it is time to push our local repository to the remote repository. In order to synchronize all our changes between the local git repository and the remote git repository, we are going to the use the <strong>push</strong> command i.e, <code>git push -u origin master \[--tags]</code> command where -u option sets up a tracking branch relationship between the master branch on the local repository and the master on the remote repository. Since the remote repository we have is named 'origin', that's the value we used. After the name/reference of the remote repository, we provide the name of the branch (we are going to push our changes from the local repository to the remote repository) which in our case is 'master'. After that, we have --tags flag to send all the tags that we currently have in our local git repository, up to GitHub (The --tags flag is optional. For the --tags flag to be considered, we type in <code>git push -u origin master --tags</code> command in the git bash). After we type in the command, we will be prompted for our GitHub Username and Password as seen below:

<pre>
Username for 'https://github.com': Ch-sriram
Password for 'https://Ch-sriram@github.com':
</pre>

After that, Git will do some house-keeping (which synchronizes the local and remote repositories) and if everything is successful, we should see an output on the terminal which is similar to the following:

<pre>
To https://github.com/Ch-sriram/Just-Git-In.git
 * [new branch]   master -> master
 * [new tag]      v1.0 -> v1.0
Branch master set up to track remote branch master from origin.
</pre>

We can see that we have two lines with <strong>\[new branch]</strong> and <strong>\[new tag]</strong> information, which means that, when we pushed our local repository to the remote repository, we created our one and only branch in the remote repository which is the 'master' branch.

We also see that we have the statement -  <strong>Branch master set up to track remote branch master from origin</strong>. This statement came up because we used the -u option when we pushed the local repository to the remote repository. In the future pushes we make to the remote repo, we need not use the -u option.

After we have pushed our local repository to the remote repository, we can check and verify our changes in the remote repository using the GitHub remote repository URL we gave earlier. 

Now when we type in <code>git status</code> in the terminal, we see the following output from git:

<pre>
On branch master
Your branch is up to date with 'origin/master'.

nothing to commit, working tree clean
</pre>

[Goto: Table Of Contents](https://github.com/Ch-sriram/Just-Git-In#table-of-contents)

## 9. SSH Authentication

Till now we used <strong>HTTPS (Hyper-Text Transfer Protocol Secure)</strong> [which is used for secure transfer communication over a computer network and is widely used in the internet] authentication with GitHub.

This time, we will set-up another authentication method known as <strong>SSH</strong> (<strong>Secure SHell</strong> is a cryptographic network protocol for operating network services securely over an unsecured network). It is recommended to use SSH when we are on a system/computer we own or a system that we use on a regular basis. SSH takes a short setup process, but once it is done, it saves a lot more time each time we make a remote change on our local repository, when compared to the HTTPS authentication. 

We will setup our SSH Key for our respective system and then save it on GitHub, so now, our account is linked via SSH authentication.

[Goto: Table Of Contents](https://github.com/Ch-sriram/Just-Git-In#table-of-contents)

### 9.1 Generating an SSH Key

The first thing we need to in order to communicate via SSH in GitHub is that we've to create an SSH key on our local system. We are currently outside the demo repository and we create a .ssh directory using <code>mkdir .ssh</code>. We will need a tool called <strong>ssh-keygen</strong> to generate both public and private SSH keys and for that, we navigate to the .ssh directory and we type in <code>ssh-keygen -t rsa -C "john.doe@example.com"</code> command where, -t option is the type of the cryptographic algorithm we are going to use, "rsa" stands Rivest-Shamir-Adleman algorithm in cryptography, -C option is for common name for which the input is the email address as shown in the command. After we press enter, we will get be prompted about where to save the file? as shown below:

<pre>
Generating public/private rsa key pair.
<strong>Enter file in which to save the key (C:/Users/srira/Desktop/.ssh/id_rsa): </strong>
</pre>

We press enter to accept the default and then we will be asked for a passphrase as shown below:

<pre>
Generating public/private rsa key pair.
Enter file in which to save the key (C:/Users/srira/Desktop/.ssh/id_rsa):
<strong>Enter passphrase (empty for no passphrase): </strong>
</pre>

We press enter to have no passphrase (it is recommended to enter the passphrase). No passphrase means that we would be asked the passphrase when we are actually linking our GitHub account to our Git repsoitory using SSH.

Now, after we enter the passphrase (or leave it empty), we will have our SSH Keys generated as the following output:

<pre>
Your identification has been saved in C:/Users/srira/Desktop/.ssh/id_rsa
Your public key has been saved in C:/Users/srira/Desktop/.ssh/id_rsa.pub
The key fingerprint is:
xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx john.doe@example.com
The key's randomart image is:
+--[ RSA 2048 ]--+
| ..             |
|..              |
|o .             |
| o .            |
|  . . . S       |
|   . E o .      |
|    = = =       |
|   = *.=        |
| .o.*o=.        |
+----------------+
</pre>

When we check the files in the .ssh directory, we should definitely have two files and they're:

<pre>
id_rsa
id_rsa.pub
</pre>

<strong>id_rsa</strong> is the private key and <strong>id_rsa.pub</strong> is our private key. We open the <strong>id_rsa.pub</strong> file in our text editor (Windows: <code>notepad id_rsa.pub</code> & Linux/Mac: <code>mate id_rsa.pub</code>) and then copy all the content of the file and then close our editor. Now we have the contents of <strong>id_rsa.pub</strong> file in our clipboard.

Now, in our internet browser, we open our GitHub Profile and go to Settings. In the Settings, we go to the menu item <strong>SSH Keys</strong>. In there, we will see that we have a functionality to add an SSH Key using the <strong>Add SSH Key</strong> button. After we press the button, we will be asked to give a <strong>Title</strong> and the <strong>Key</strong>. In the <strong>Title</strong> field, we will give a description of the SSH Key we are using as an SSH Key is usually associated with some system/computer (example: My Lenovo YogaPad \[PC]) and then we will paste the contents of the clipboard into the Key field and then press <strong>Add key</strong> button. After that, GitHub prompts us for password of the GitHub account so that we can get into <strong>super user mode</strong>. Once we have successfully authenticate using our GitHub password, we will be redirected to the SSH keys sub-menu in Personal settings menu where we will see our SSH key with the title we gave alonf with the public key. We can always delete the SSH Key we have from that same menu using the Delete button.

Now to confirm whether the machine we generated the SSH Key on is able to communicate with GitHub via SSH, we are going to use the SSH command to try to login. For that we type in <code>ssh -T git@github.com</code> in the terminal inside the .ssh directory, and we should something similar to the following output in the terminal:

<pre>
The authenticity of host 'github.com (192.30.234.66)' can't be established
RSA key fingerprint is xxxxxxxxxxxxxxxxxxxxxxxx.
Are you sure you want to continue (yes/no)? 
</pre>

We will be given a prompt as shown above and we should type in <strong>yes</strong> and we will be prompted again for our SSH Key Password. We have the option to remember the SSH Key Password depending on the Operating System we are using. We type in the SSH Key Password and then click "OK" and we should see the following output in the terminal:

<pre>
Identity added: C:/users/srira/Desktop/.ssh/id_rsa (C:/users/srira/Desktop/.ssh/id_rsa)
Hi Ch-sriram! You've successfully authenticated, but GitHub does not provide shell access.
</pre>

[Goto: Table Of Contents](https://github.com/Ch-sriram/Just-Git-In#table-of-contents)

## 10. GitHub Repository

We will know how to apply local operations in a git repository, but by using the GitHub Interface. We will view, edit, create & delete files all directly on the GitHub interface.

We will also go over the unique aspects of the GitHub's remote repository and how it relates to our local repositories back on our system. 

While we can make smal changes in our project using the GitHub Interface, but the more significant changes are recommended to be done using the Git CLI (or the git bash).

We can create a repository on GitHub from the steps given [here](https://help.github.com/en/enterprise/2.13/user/articles/creating-a-new-repository).

[Goto: Table Of Contents](https://github.com/Ch-sriram/Just-Git-In#table-of-contents)

### 10.1 Cloning a GitHub Repository

We can clone a GitHub Repository easily from the repository link (link can be an SSH or HTTPS link) itself. Whenever we open a GitHub repository in the github's website in the web browser, we can see an option in the repository which has information on the <strong>clone URL</strong> by pressing the <strong>Clone or download</strong> button. We have two types of URLs to choose from, one is HTTPS, another is SSH. We can choose either. We will choose SSH URL. We will copy the SSH URL of the the respective GitHub Repository and in our terminal, we type in the <strong>clone</strong> command with the following syntax: <code>git clone clone-url \[directory-name]</code> (example: If we use the command w/o giving the optional \[directory-name] option, then we will clone the directory from GitHub to our local machine with the same name as the repo's name and so the command would be the following: <code>git clone git@github.com:Ch-sriram/Practice-CPP.git</code>. Otherwise, if we want a custom directory name, we would give the optional \[directory-name] option which is <code>git clone git@github.com:Ch-sriram/Practice-CPP.git CPP</code>).

After we clone the repository, we can see that the contents inside the clones repository is the same as that of the files list we saw inside the remote repository hosted on GitHub. Inside the cloned repository, whenever we type in <code>git remote -v</code>, we will see that the git repository is automatically connected to GitHub via SSH with both the fetch and pull links having the same URL as seen below:

<pre>
origin git@github.com:Ch-sriram/Practice-CPP.git (fetch)
origin git@github.com:Ch-sriram/Practice-CPP.git (push)
</pre>

[Goto: Table Of Contents](https://github.com/Ch-sriram/Just-Git-In#table-of-contents)


### 10.2 Fetch & Pull in GitHub

Right now, we are in our [CPP repository](https://github.com/Ch-sriram/Practice-CPP) (which we cloned earlier) in the web browser, and while we are in the repository, we are going to make a quick change in the repository directly through the github website. We are going to open the README.md file in the repository and then edit that file (Note that the CPP repository should be a part of our repositories in our respective GitHub account to edit on GitHub). After editing/adding some content in README.md, we can provide the Commit Message and the provide optional extended description and then we can choose if we want to <strong>Commit directly to the <code>master</code> branch</strong> or create a new branch for the commit and start a pull request. We will simply make the commit on the master branch, and then press the <strong>Commit changes</strong> button. 

Now we just updated our remote repository, a change of which our local repository is currently unaware of. In our local repository, in the terminal, when we check the status of our repository (which is CPP repo) using <code>git status</code>, we will see the following output in the terminal:

<pre>
On branch master
Your branch is up-to-date with 'origin/master'

nothing to commit, working directory clean
</pre>

While we are in the CPP repository, we can make some changes to the README.md file there, and then commit our changes using the express commit, i.e., using <code>git commit -am "README Update"</code> command and we should see house-keeping output. Now when we check the status of CPP repository using <code>git status</code> command in the terminal, we would see the following output:

<pre>
On branch master
Your branch is ahead of 'origin/master' by 1 commit.
  (use "git push" to publish your local commits)
nothing to commit, working directory clean
</pre>

Now according to the message seen above, we can see that we are ahead of the remote repository by 1 commit, however, we know that we have made a commit in CPP remote repository through the GitHub website and therefore, if we now try to publish the changes made in the local repository to the remote repository using <code>git push</code>, we'd get the following output in the terminal:

<pre>
To github.com:Ch-sriram/Practice-CPP.git
 ! [rejected]        master -> master (fetch first)
error: failed to push some refs to 'git@github.com:Ch-sriram/Practice-CPP.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
</pre>

When we tried to publish our changes in the local repository to the remote repository, git has rejected the push because we have made a commit in the remote repository and we have to first <strong>fetch</strong> the changes we made in our remote repository and then <strong>merge</strong> those changes to our local repository, otherwise, we can simply <strong>pull</strong> the changes from the remote repository to the local repository which will <strong>fetch + merge</strong> at the same time. But when pulling (or merging in general) there's obviously a possibility that the pull might fail due to a merge conflict (in that case, we go to a MERGING state and then use our mergetool to resolve the merge conflict), but most oftenly, the pull request goes in automatically (due to a fast-forward merge).

Now, if we are not sure whether there'll be merge conflict or not, we generally go for <strong>fetching</strong> and then <strong>merging</strong> the remote repo changes into our local repo manually rather than going for the <strong>pull</strong> command, which can be a destructive command if we have changes that are not compatible with what currently is in the remote repository.

Therefore, we alleviate the usage of pull by using the <strong>fetch</strong> command, i.e., using <code>git fetch</code> command in the terminal, and we should see something similar to the following output:

<pre>
remote: Enumerating objects: 5, done.
remote: Counting objects: 100% (5/5), done.
remote: Compressing objects: 100% (3/3), done.
remote: Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), 717 bytes | 4.00 KiB/s, done.
From github.com:Ch-sriram/Practice-CPP
   56b8dac..fdcf788  master     -> origin/master
</pre>

Now when we check the status using <code>git status</code> command, git responds with the following output in the terminal:

<pre>
On branch master
Your branch and 'origin/master' have diverged,
and have 1 and 1 different commits each, respectively.
  (use "git pull" to merge the remote branch into yours)

nothing to commit, working tree clean
</pre>

We can see that the message depicts that we have 1 commit from local and 1 commit from the remote repository. Also, the message says that we can merge the changes automatically using <code>git pull</code> command in the terminal. Now when we type in <code>git pull</code> command in the terminal, since the master branch on both sides (remote and local) are different, what occurs is a merge commit and so, we will see a MERGE_MSG file open where we type in the commit message we want. By default, the commit message we will see is - <strong>Merge branch 'master' of github.com:Ch-sriram/Practice-CPP</strong> which is a perfectly fine commit message. Therefore, we leave the message as that and then save and close the editor where the MERGE_MSG file was opened and then we publish the changes to GitHub using <code>git push</code> and we should get an output which is house-keeping output.

Doing a <strong>pull</strong> or a <strong>fetch</strong> prior to any <strong>push</strong>es is the best practice when trying to publish the changes made in the local repository to our remote repository.

We can verify our changes in GitHub in our CPP repository.

[Goto: Table Of Contents](https://github.com/Ch-sriram/Just-Git-In#table-of-contents)


### 10.3 Updating Remote References of a Repository

We will be in need of updating our remote references of the local repository when we rename the repository, because the SSH/HTTPS URL changes with respect to the name of the repository. Please know how to rename a repository [here](https://help.github.com/en/github/administering-a-repository/renaming-a-repository). Assume that we renamed <strong>Practice-CPP</strong> to <strong>CPP</strong>.

After renaming our repository, we generally have to change our remote reference to the local repository, because that particular remote reference is not functional anymore. When we check the remote reference our local repository is connected to using <code>git remote -v</code> command, we get the following output:

<pre>
origin  git@github.com:Ch-sriram/Practice-CPP.git (fetch)
origin  git@github.com:Ch-sriram/Practice-CPP.git (push)
</pre>

Now, that we have renamed our repository, we need to update the remote reference to origin by copying the clone URL (SSH or HTTPS, depending on what you want) and then using <code>git remote set-url origin git@github.com:Ch-sriram/CPP.git</code> command in the terminal and then we check the remote reference again using <code>git remote -v</code> command in the terminal and we should see the following output:

<pre>
origin  git@github.com:Ch-sriram/CPP.git (fetch)
origin  git@github.com:Ch-sriram/CPP.git (push)
</pre>

We can get additional information about our remote reference by typing in <code>git remote show origin</code> command (where 'origin' is the name of the remote reference) in the terminal and we should get a similar output as shown below:

<pre>
* remote origin
  Fetch URL: git@github.com:Ch-sriram/CPP.git
  Push  URL: git@github.com:Ch-sriram/CPP.git
  HEAD branch: master
  Remote branch:
    master tracked
  Local branch configured for 'git pull':
    master merges with remote master
  Local ref configured for 'git push':
    master pushes to master (up to date)
</pre>

We can see more information related to the remote reference and we see that the Remote branch is master and it is <strong>tracked</strong>, which means whenever we do a <code>git push</code> or <code>git pull</code>, git will automatically synchronize between the master branches on both sides (viz. remote and local).

[Goto: Table Of Contents](https://github.com/Ch-sriram/Just-Git-In#table-of-contents)


### 10.4 Creating New Files in GitHub on a New Branch

In our CPP repository on GitHub (which is [here](https://github.com/Ch-sriram/Practice-CPP)), we will create a new file by clicking on the <strong>Create new file</strong> button in the repository page in the web browser. We can go into any sub-directory inside our GitHub repository and create a new file by giving a name to the file with the appropriate extension and then typing in the content of the file in the <strong>Edit new file</strong> section. After we fill the content inside the file, we can also preview the file before committing the changes by clicking on the <strong>Preview</strong> tab beside the <strong>Edit new file</strong> tab in the web browser.

After we fill the content in the new file, we scroll to the bottom of the webpage and then put in our commit message's title along with any additional optional description (if we want, we can put in the description in markdown syntax) and then we can <strong>commit directly to the <code>master</code> branch</strong> or we can <strong>Create a <u>new branch</u> for this commit and start a pull request</strong>. We will create a new branch for the commit and start a pull request. We will name our branch <strong>feature-branch</strong> and we click on <strong>Propose new file</strong> button.

We will be redirected to <strong>Open a pull request</strong> page where we are effectively making a pull request into our master branch in the remote repository itself. We can edit the commit message we gave earlier while committing the creation of the new file, or leave it as it is. After the pull request commit message we have a comment that will go along with it where we can drop-in images and use markdown there too. After we finish with the commit message and the comment, we can simply press the <strong>Crete pull request</strong> button. 

We will see a message which says <strong>This branch is up-to-date with the base branch</strong> and since we are the only contributor of the repository, we will click the <strong>Merge pull request</strong> button below the message. We will again have the opportunity to modify the commit message prior to clicking on <strong>Confirm merge</strong> button. Once we've clicked the button, we will be shown one more message which says <strong>Pull request successfully merged and closed</strong> and we will have a button beside it which is <strong>Delete branch</strong> and we can click that button to delete the branch ("feature-branch") that we created earlier. We click <strong>Delete branch</strong> button and we delete the branch we created earlier.

To verify the changes made, we go to CPP repository home and we check that the newly created file is there in the remote repository.

[Goto: Table Of Contents](https://github.com/Ch-sriram/Just-Git-In#table-of-contents)


### 10.5 Synchronizing Changes made in Remote Repository to the Local Repository

After we made the changes in the remote repository as we have seen in the section above (in 10.4), now we have to synchronize the changes that we made in the remote repository into our local repository. For that, we type in <code>git fetch</code> in the terminal, and we will see an output which is of the following sort:

<pre>
remote: Enumerating objects: 5, done.
remote: Counting objects: 100% (5/5), done.
remote: Compressing objects: 100% (4/4), done.
remote: Total 4 (delta 1), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (4/4), 1.64 KiB | 6.00 KiB/s, done.
From https://github.com/Ch-sriram/Just-Git-In
   05dd1ca..1a54600  master     -> origin/master
</pre>

Now if we check the status using <code>git status</code> command in our demo repository, we will see the following output:

<pre>
On branch master
Your branch is behind 'origin/master' by 2 commits, and can be fast-forwarded.
  (use "git pull" to update your local branch)

nothing to commit, working tree clean
</pre>

Now we can simply type in a <code>git pull</code> in the terminal, and we shall an output that's similar to the following:

<pre>
Updating 05dd1ca..1a54600
Fast-forward
 lorem.txt | 4 ++++
 1 file changed, 4 insertions(+)
 create mode 100644 lorem.txt
</pre>

Now when we check the status (using <code>git status</code> command) of our demo repository, we will see the following output:

<pre>
On branch master
Your branch is up to date with 'origin/master'.

nothing to commit, working tree clean
</pre>

Now when we type in <code>ls</code> in our terminal, we will see that <strong>lorem.txt</strong> is in our local repository as seen below:

<pre>
app.log  LICENCE.txt  lorem.txt  README.md
</pre>


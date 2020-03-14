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
   8. [Rolling Back Changes]()
   9. [Creating New Commands - Git Alias]()
   10. [Renaming & Deleting Files Using Git Bash]()
   11. [Renaming & Deleting Files Not Using Git Bash, but the OS Commands]()
   12. [Excluding/Ignoring Unwanted Files in our Git Repository]()
7. [Advanced Version Control Using Git]()
   1. [Introduction]()




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


### 6.8 Rolling Back Changes
Here, we will back out the changes we made previously by unstaging our changes from the git staging area and then finally we will revert our changes entirely. 

In our "demo" git repository, when we git bash the command <code>git status</code>, we can see that there will be nothing to commit and we will see the following message: <em>nothing to commit, working directory clean</em>.

Now, we will modify the README.md file again and we will put some random text inside it. We save and close the README and then we again type in <code>git status</code> command inside the git bash. We can see that we will have the message - <strong>modified: README.md</strong> and then we can add the changes into the repository using <code>git add .</code> command in our git bash. When we type in <code>git status</code> again, we can see that we see the message - <strong>Changes to be committed: modified: README.md</strong> in the git bash. 

Now, to unstage the changes, or undo the commit, we can type in the command <code>git reset HEAD README.md</code> where README.md is the file to be unstaged from the user's repository. When we open up our README.md file, the changes that we made, will still be there, but the changes that we made have simply been unstaged, that means, when we type in the command <code>git status</code>, we can see that the message we get is - <strong>Changes not staged for commit: modified: README.md</strong> in the git bash.

Now, if we don't want the changes that we made and to discard the changes made to the repository, we can simply revert back to the last known good state (or commit) of the respective file (here, it is README.md) whose details are available inside the .git folder, we simply type in <code>git checkout -- &lt;file-name></code> (ex: <code>git checkout -- README.md</code>). Now, we can check the status of the repository with <code>git status</code> command, which will respond with the message - <em>nothing to commit, working directory clean</em> in the master branch of our "demo" repository. Now if we open README.md, we can see that the changes we made are also gone.


### 6.9 Creating New Commands - Git Alias
We will create a git alias to shorten a command into a smaller command. In our "demo" repository, in the master branch, when we type in <code>git status</code>, we can see that we have <em>nothing to commit, working directory clean</em> as the message. Now to see the options available with the <code>git log</code> command, we can simply type in <code>git help log</code> command.

Out of all the options available, we can type in the log command as <code>git log --oneline --graph --decorate --all</code> where <strong>--online</strong>: provides a simplified commit entry providing the log information in a single line instead of multiple lines, <strong>--graph</strong>: provides an asterisk(*) based graph denoting our branching hierarchy, <strong>--decorate</strong>: tells us which commits are part of which branches, <strong>--all</strong>: provides the history for all the branches that are available in the repository. We will see an output in git bash which will show us the entire history of our significant commits. Now, whenever we want to get details in this manner, we always have to type in <code>git log --oneline --graph --decorate --all</code> command every time. Instead of typing it all the time, we can use <strong>git aliases</strong>.

To create a git alias (which is basically a new command in git bash and a shortened representation of an existing combination of longer command(s)) we will type in <code>git config --global alias.hist "log --oneline --graph --decorate --all"</code> command in the git bash and we have created an alias for the above command called "hist". So whenever we want to call the longer command, we can simply type in <code>git hist</code>. To check our list of aliases that we have configured in git configuration, we simply type in <code>git config --global --list</code> command in the git bash.

Using aliases, we can also add more options to the underlying command, it simply replaces the alias command with the actual command and concatenates the options that we added. For example, the command <code>git hist -- LICENCE.md</code>, will convert into the actual command which is <code>git log --oneline --graph --decorate --all -- LICENCE.md</code>, where the command will give us all the commit logs related to LICENCE.md file in the repository.


### 6.10 Renaming & Deleting Files Using Git Bash
In our demo repository, we will create a file called <strong>example.txt</strong> and insert some random text into the file and save and return back to the git bash. We type in <code>git status</code> and check the status of our git repository and we will see the message <strong>Untracked files: example.txt</strong>. We will add the new file using <code>git add example.txt</code> command in git bash. Finally, we commit the changes made into the repo using <code>git commit -m 'adding example.txt'</code>. When we list the files in the git bash using <code>ls -la</code> command, we will see that we have the three files <strong>LICENCE.md, README.md & example.txt</strong> in our repository. 

Now, if we want to change the name of the file we just made, we can change the name in the git bash using the <code>git mv example.txt demo.txt</code> command. When we again check the status of the repository (using <code>git status</code> command), we will see the message - <strong>Changes to be committed: renamed:     example.txt -> demo.txt</strong>. This change is in the staged state. The renaming takes effect properly, only when we commit. When we list the files of the repository (using <code>ls -la</code> command) in git bash, we can see that the file has already been renamed on the Operating System. But to finish the task, we need to actually commit the changes and let our changes be in the .git directory, in the final state, the Committed State. For that, we type in <code>git commit -m "renamed example.txt to demo.txt"</code>. We will see a message - <strong>rename example.txt => demo.txt (100%)</strong> where the 100% inside the parentheses is the confidence level given by git that this file's content is a 100% similar to the previous file name, i.e., example.txt's context hasn't been changed, only the name of the file has been changed to demo.txt. If we would've made modifications to demo.txt before committing the state of the repository, then the confidence level would've been lower than 100%.

If we wanted to delete a file that we made, we can remove it using the <code>rm</code> command in the git bash. To remove it using the git bash (instead of the facilities provided by the OS), we type in <code>git rm demo.txt</code> command in the git bash. If we delete/rename/modify files using the git commands (instead of the commands provided by the OS), we will get the additional benefit of git tracking the changes that we made in our repository. And so, we will have more power with us using the version control system. Now, if we simply list the files in our repository, we will see that we no longer have demo.txt file in our repository. Now, when we check the status of our repository (using <code>git status</code> command), we can see the message - <strong>Changes to be committed: deleted:    demo.txt</strong>, meaning, our deletion is just staged, it hasn't been committed. Therefore, we have to commit to completely reflect the changes in the .git directory of our repository using <code>git commit -m "deleting demo.txt file"</code>. When we check the status of our repo, we should see the message <em>nothing to commit, working directory clean</em>.


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


### 6.12 Excluding/Ignoring Unwanted Files in our Git Repository
Assume that we create a new log file inside our demo repository (Windows: <code>notepad app.log</code> & Linux/Mac: <code>touch app.log</code>). When we check the status of the git repository, we will see that the newly created log file is untracked, and the message we should get is - 

<pre>
Untracked files:
      <strong>app.log</strong>
</pre>

In general, in a repository, we don't want anything other than the source code of the app that we are developing. Therefore, log files, images, videos, etc are not supposed to be in our git repository. For this, our version control, i.e., git, has to ignore these files. To exclude files/folders that we don't want in our git repository, we create a <strong>.gitignore</strong> file inside which we write the relative paths of the files that we don't want to be tracked in our repository.

Therefore, we create a <strong>.gitignore</strong> file in cmd/terminal (Windows: <code>notepad .gitignore</code> & Linux/Mac: <code>touch .gitignore</code>) and then type in the relative path of the file/folder that we want to completely exclude from being tracked by the git version control. In our case, we want to exclude app.log file, and therefore, in our .gitignore file, we can type in the following - 
<strong><em>.gitignore</em></strong>
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



## 7. Advanced Version Control Using Git
In this section, we will learn more advanced concepts and techniques in git that apply in local repository. Some of the topics covered in this section include: the following topics:
- Comparing Differences,
- Branching, Merging & Conflict Resolution,
- Marking Milestones w. Tagging,
- How to save Work in Progress,
- How to Time Travel, Other, etc.



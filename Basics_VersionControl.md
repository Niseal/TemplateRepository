

[Source with Images](https://adamtheautomator.com/visual-studio-code-github/)
[Video on Basics](https://www.youtube.com/watch?v=F2DBSH2VoHQ)



## In Short:

### Does VS Code recognise Git? / Your Configuration?

'git --version'
'git config --list'

### Configuring Git (only required once)

'git config --global user.name "Niseal"'
'git config --global user.email "n.broekmeijer@live.nl"'

### Using Git \(Locally\) 

Source Control \(view sidebar\), shortcut CTRL\+SHIFT\+G

### Linking Repositories \(Remotely\)

We create a local directory in Visual Studio Code and a repository in Github, then either Clone the Github repository in VS code or Push the working directory to Github
This requires atleast one file in either the Github repository (if Github -> VS Code) or the local directory (if VS Code -> Github)

##### From Github -> VS Code

Clone Repository in VS Code Source Control tab

  IF Source Control is empty:
     Source Control -> Clone Repository -> Clone from GitHub -> … -> Search / Select Repository -> Specify destination -> Login -> Open

  IF Source Control isn't empty:
     Source Control -> More Actions \(…\) -> Clone -> Search / Select Repository -> Specify destination -> Login -> Open

#### From VS Code -> Github

Open Folder in VS Code Source Control tab

  IF Source Control is empty:
     Source Control -> Open Folder -> Select Folder -> Publish to Github -> Login -> Specify Repository Type -> Select Files -> Open

  IF Source Control isn't empty:
     Source Control -> More Actions \(…\) -> Clone -> Search / Select Repository -> Specify destination -> Login -> Open


1. Create new / open existing repository in GitHub

2. Clone Github repository in VS Code Source Control tab

3. Create local branch / Navigate branches in status bar (branch logo)

4. Create / Edit files in Explorer view, **Save files with CTRL\+S**

5. Review changes in Source Control view, then either Discard ↶ or \+ Save changes

6. Commit changes to local repository in Source Control view, by writing a message and clicking the commit button ✓ 

7. Push changes to remote repository in Source Control view, by through More Actions … -> Push


## High\-Level Introduction


### Working on Files

To start working on a file or program from scratch, you can create a new file in the "File" menu, \(shortcut CTRL\+N\). This is also where you can open local files \(shortcut CTRL\+O\), or open a local directory \(shortcut CTRL\+K CTRL\+O\). When working on your programs or files, you'd preferably do so from within the "Explorer" view \(shortcut CTRL\+SHIFT\+E\). The Explorer view gives an overview of all the files in the working (local) directory, quick access to all these files and some basic shortcuts in the UI. 

### Using Git \(Locally\)

Git is used for \(local\) version control. Its main use is keeping track of the development of a file / workspace you are working on. It gives insight in the changes that have been made up to this point, and offers the possibility to revert back and compare changes before they are finalized. This is done through 'branches'. There is always a 'main' \(or 'master'\) branch, which is the 'stable' version of a file, and 'ofshoots', which represent changes that haven't been integrated with the main branch yet. The best way to make use of this configuration is to make a new branch for every atomic change that is to be made to the main branch, work on these changes in the new branch, and 'merge' them with the main branch whenever it's clear that everything works as expected. Git also allows for \(local\) collaboration, and does so with 'Push' and 'Pull' requests. Git keeps snapshots of all files associated with it, which can differ from local copies of collaborators, and can be seen as the 'consensus' between all local collaborators. This consensus can be updated through push requests, through which a collaborator can request that his local copy of a branch becomes the new consensus. As the consensus can change (and local copies aren't updated automatically), pull requests are used to update local copies of collaborators with respect to the consensus. 

In Visual Studio Code, Git can be accessed through the "Source Control" View button, or its shortcut, CTRL\+SHIFT\+G.

### Extending Git with Github \(Remote\)

In essence Github does the same as Git, but it extends these capabilites to a remote server, making it possible to use this Version Control System remotely. This adds the possibility to collaborate on a project from remote locations, or access a personal project from different locations. 

In Visual Studio Code, Github can be accessed through the "Github" View button.



## Git in practice


### Logging In

'git config --list'
'git config --global user.name "Niseal"'
'git config --global user.email "n.broekmeijer@live.nl"'

### Navigating and Creating Branches

By default, you start in the main \(or: master\) branch in your local repository. This is shown on the left side of the **status bar**, next to the branch icon. To **create** a new local branch or **navigate** existing branches, click on the **branch icon** and navigate through the command palette options.

### Adding and Modifying Files

Files can be added and edited from the **explorer** view. To add a new file to the workspace, press CTRL\+N or go to File —> New File. New files are marked with a **U**, meaning they are **untracked**. Untracked files are any files in your working directory that were not in your last snapshot and are not in your staging area. An edited file will be marked by an **M**, which stands for **modified**. Other markings are **D** for **deleted** and ...? **Dont forget to save your files with CTRL\+S**

### Reviewing and Staging Changes

To look at and review the changes, go to the **Source Control** view. After reviewing, you are expected to either discard or stage the changes to the files, by clicking on the **discard \(↶\)** or the **stage \(\+\)** sign next to the filename. When changes are staged, the \+ icon becomes a \- icon, which can be used to **unstage** changes. You can also stage or discard all changes at once by clicking on the **More actions \(…\)** button and selecting either the **Stage All Changes** or **Discard All Changes** menu items. 

### Committing Changes

Now that the changes have been staged, the next action is to **commit** the changes **to the local repository**. To commit the changes, you must include a meaningful message in the **message bar**. Once you’re satisfied with your message, press CTRL\+ENTER or click the commit \(✓\) button to finish saving the changes to the local repository. 



## Github in Practice


### Publishing local branches

The **cloud icon** right next to the branch icon is used to **publish changes**. This is necessary when a (newly created) local branch has no equivalent in the Github repository (upstream branch). Publishing changes creates the local branch in the remote repository, and pushes its content.

### Pushing Changes to GitHub

After changes are saved to the local repository, the **Source Control** view should reflect that the number of changes has reset to zero (0). To finally **push** the changes in the local repository **to remote repository** in GitHub, click on the **More actions \(…\)** button and then click on **Push**.

### Pulling Changes from Github



### Cloning a GitHub Repository

First, click the **Source Control** view button or press the keyboard shortcut CTRL\+SHIFT\+G. Next, click the **Clone Repository** button. Then, click on Clone from GitHub, and you will be prompted to allow a sign-in attempt. Click on **Allow**. 

The authorization page will automatically launch in your default web browser. Click on the **Continue** button.

The next page shows you the permission request details. To proceed in giving VS Code the required permissions, click on the **Authorize GitHub** button.

When authorization is done, you will get a status page. If prompted that the site is trying to open Visual Studio Code, click **Open**.

Once you’re back in the VS Code window, you can either **search** of the repository name or **select** the repository name that you intend to clone in the command palette. 

After selecting the repository to clone, you will be asked to provide the folder where the repository will be saved locally on your computer. Specify the destination folder and click on **Select Repository Location**.

>Note: GitHub log in will be triggered when performing actions that require authentication. Such actions include cloning from a private repository or pushing to a repository

The **GitHub Login** window will pop up, and you need to enter your GitHub credentials to log in.

After completing the login, VS Code will proceed to clone the remote repository to your computer. Once the cloning is done, you would get a notification at the bottom right of the VS Code window. Now, you can click either **Open** or **Open in New Window** depending on your preference.

### Opening a local directory in Github


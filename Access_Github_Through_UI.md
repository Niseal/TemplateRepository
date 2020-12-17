[Source with Images](https://adamtheautomator.com/visual-studio-code-github/)

## In Short:
1. Create new repository in GitHub

2. Clone Github repository in VS Code

IF Source Control is empty:
   Source Control -> Clone Repository -> Clone from GitHub -> … -> Search / Select Repository -> Specify destination -> Login -> Open -> **DONE** 

IF Source Control isn't empty:
   Source Control -> More Actions \(…\) -> Clone -> Search / Select Repository -> Specify destination -> Login -> Open -> **DONE**  

3. Create / Edit files in Explorer view, **Save files with CTRL\+S**

4. Review changes in Source Control view, then either Discard ↶ or \+ Save changes

5. Commit changes to local repository in Source Control view, by writing a message and clicking the commit button ✓ 

6. Push changes to remote repository in Source Control view, by through More Actions … -> Push



## Cloning a GitHub Repository

First, click the **Source Control** view button or press the keyboard shortcut CTRL\+SHIFT\+G. Next, click the **Clone Repository** button. Then, click on Clone from GitHub, and you will be prompted to allow a sign-in attempt. Click on **Allow**.

The authorization page will automatically launch in your default web browser. Click on the **Continue** button.

The next page shows you the permission request details. To proceed in giving VS Code the required permissions, click on the **Authorize GitHub** button.

When authorization is done, you will get a status page. If prompted that the site is trying to open Visual Studio Code, click **Open**.

Once you’re back in the VS Code window, you can either **search** of the repository name or **select** the repository name that you intend to clone in the command palette. 

After selecting the repository to clone, you will be asked to provide the folder where the repository will be saved locally on your computer. Specify the destination folder and click on **Select Repository Location**.

>Note: GitHub log in will be triggered when performing actions that require authentication. Such actions include cloning from a private repository or pushing to a repository

The **GitHub Login** window will pop up, and you need to enter your GitHub credentials to log in.

After completing the login, VS Code will proceed to clone the remote repository to your computer. Once the cloning is done, you would get a notification at the bottom right of the VS Code window. Now, you can click either **Open** or **Open in New Window** depending on your preference.


## Staging, Committing and Pushing Changes to GitHub

### Adding and Modifying Files

Files can be added and edited from the **explorer** view. To add a new file to the workspace, press CTRL\+N or go to File —> New File. New files are marked with a **U**, meaning they are **untracked**. Untracked files are any files in your working directory that were not in your last snapshot and are not in your staging area. An edited file will be marked by an **M**, which stands for **modified**. **Dont forget to save your files with CTRL\+S**

### Reviewing and Staging Changes

To look at and review the changes, go to the **Source Control** view. After reviewing, you are expected to either discard or stage the changes to the files, by clicking on the **discard \(↶\)** or the **stage \(\+\)** sign next to the filename. You can also stage or discard all changes at once by clicking on the **More actions \(…\)** button and selecting either the **Stage All Changes** or **Discard All Changes** menu items. 

### Committing Changes

Now that the changes have been staged, the next action is to **commit** the changes **to the local repository**. This step comes before pushing the changes to the remote GitHub repository. To commit the changes, you must include a meaningful message in the **message bar**. Once you’re satisfied with your message, press CTRL\+ENTER or click the commit (✓) button to finish saving the changes to the local repository. 

### Pushing Changes to GitHub

After the changes are saved to the local repository, the **Source Control** view should reflect that the number of changes has reset to zero (0). To finally **push** the changes in the local repository **to remote repository** in GitHub, click on the **More actions \(…\)** button and then click on **Push**.




[Interactive Markdown Cheat Sheet](https://www.markdownguide.org/cheat-sheet/)

#### Cheat Sheet in Short:

###### Heading

\#              H1
\#######        H6


CheatSheet - Setup Github on Visual Studio Code

Steps:

    Create a directory on the local file system.
    Create a repo on Github.
    Select Clone "Clone or download" on Github, copy the link
    In Visual Studio Code, sect File -> Add Folder to Workspace -> Select the newly created directory
    Select Terminal Window
    In the window, type:

git config --global user.name <github userID>

git clone <URL from github link copied earlier>

That should be all that's required.  any newly created file should be available on github after stage/commit/push.

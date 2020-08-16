# Creating a Repository Using Git Bash

Open Git Bash. <br>
Navigate to a folder where you would want to create your repo.
![Creating Repo using Git Bash](/Assets/Creating%20Repo%20in%20Git%20Bash.png)

Shortcut - Open the folder in File Explorer & right Click o empty space and click on "Git Bash Here"

![Creating Repo using Right click](/Assets/Creating%20Repo%20in%20Git%20Bash%20using%20Right%20click.png)
<br><br>
To initialize the repo, run this command <br>
`git init`
<br>

### Using existing repo

The method is same. You have to just navigate inside Git Bash. There will be no need to initialize as you have already done it. Use this command to check current status.<br>
`git status`

<br> For this Guide, I will be using the Demo Repo which we created earlier.

##### Incase you want to use repo from your GitHub account

Copy the WebURL (ending with .git)<br>
_In this picture, it is not showing completely. Just use that copy button._
![Copying GitHub Repo WebURL](/Assets/Cloning%20Repo%20into%20GD.png)

And use the command <br>
`git clone <url>`

![Cloning repo via Git Bash](/Assets/Git%20bash%20clone.png)

**Note:** After cloning, you need to enter into the local repo folder. Use `dir` command to list all the folders present. Use `cd` command to enter inside your repo.

#### Adding files & other stuff

There are few linux terminal commands which work in Git Bash. And some Windows CMD commands too. In the above screnshots you can observe that `dir` is Windows CMD command & it works. Equivalent linux terminal command is `ls`. <br><br>
My point is, you can use the usual linux terminal command to navigate & copy files.<br><br>
For the sake of simplicity, I will not be using terminal/CMD commands to copy files. I will be using Windows File Explorer to copy the files, Atom Text editor to edit them & finally Git Bash to commit changes.<br>

I will be using both the repos - <br>
`Demo-repo`  (This one is hosted on GitHub)<br>
`Gitbash repo` (This one is locally created Repo)<br>
To show how it is done.<br>

![Empty GitBash Repo](/Assets/Empty%20Gitbash%20Repo.png)

After Adding a sample text file -<br>
![GitBash Repo with sample txt file](/Assets/GBR%20with%20sample%20txt.png)<br><br>

As you can see in the screenshot, the command for adding files for tracking is -<br>
`git add <complete file>`

The file name should be enclosed in quotation marks if it contains any spaces.

Simply putting the command yields this result-<br>
`Nothing specified, nothing added.`

_Pro tip_ - Use double quotes every time (even if there are no spaces in filename) to prevent any headaches & errors. In this way it is guaranteed that your file will be taken as input properly.<br>

Repeat this command for all the files/folders you copied to the repo.

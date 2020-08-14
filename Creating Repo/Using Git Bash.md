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

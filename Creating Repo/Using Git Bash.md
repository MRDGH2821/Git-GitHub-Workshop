# Creating Repo Using Git Bash

Here we face 2 scenarios.

1.  Creating/Using locally created new/existing Repository.
2.  Creating/Using GitHub created new/existing Repository.

While Initial steps differ, but once the repo is initialized, steps are same for all given scenarios.

## Scenario 1: Creating/Using locally created new/existing Repository.

### Creating a local Repository

Open Git Bash. <br>
Navigate to a folder where you would want to create your repo.
![Creating Repo using Git Bash](/Assets/Creating%20Repo%20in%20Git%20Bash.png)

Shortcut - Open the folder in File Explorer & right Click o empty space and click on "Git Bash Here"

![Creating Repo using Right click](/Assets/Creating%20Repo%20in%20Git%20Bash%20using%20Right%20click.png)
<br><br>
To initialize the repo, run this command <br>
`git init`
<br>

### Using existing Repository

The method is same except the creation part. Navigate to the local Repo folder inside Git Bash.

Use this command to check current status.<br>
`git status`

## Scenario 2: Creating/Using GitHub created new/existing Repository.

### Creating new GitHub Repository.

Click/Tap [here](www.github.com/new) to create a new GitHub Repository.<br>

Or open your GitHub profile and create from there.<br>

After creating, Copy the WebURL (ending with .git)<br>
_In this picture, it is not showing completely. Just use that copy button._
![Copying GitHub Repo WebURL](/Assets/Cloning%20Repo%20into%20GD.png)

And use the command <br>
`git clone <url>`

![Cloning repo via Git Bash](/Assets/Git%20bash%20clone.png)

**Note:** After cloning, you need to enter into the local repo folder. Use `dir` command to list all the folders present. Use `cd` command to enter inside your repo.

### Using existing GitHub Repository.

Open your GitHub profile and Instead of creating a new Repo, open the repo where you wish to upload your code.<br>

Rest of the steps are same as above.<br><br><br>

**_Common steps_**<br>

## Adding files & other stuff

There are few linux terminal commands which work in Git Bash. And some Windows CMD commands too. In the above screnshots you can observe that `dir` is Windows CMD command & it works. Equivalent linux terminal command is `ls`. <br><br>
My point is, you can use the usual linux terminal command to navigate & copy files.<br><br>
For the sake of simplicity, I will not be using terminal/CMD commands to copy files. I will be using Windows File Explorer to copy the files, Atom Text editor to edit them & finally Git Bash to commit changes.<br>

I will be using both the repos - <br>
`Demo-repo`  (This one is hosted on GitHub)<br>
`Gitbash repo` (This one is locally created Repo)<br>
To show how it is done.<br>

![Empty GitBash Repo](/Assets/Empty%20Gitbash%20Repo.png)

#### Staging the Files

After Adding a sample text file -<br>
![GitBash Repo with sample txt file](/Assets/GBR%20with%20sample%20txt.png)<br><br>
The new files are currently unstaged. We need to move them to staging area where we can commit them & push the changes.<br>

As you can see in the screenshot, the command for adding/Staging files for tracking is -<br>
`git add <complete file>`

The file name should be enclosed in quotation marks if it contains any spaces.

Simply putting the command yields this result-<br>
`Nothing specified, nothing added.`

_Pro tip_ - Use double quotes every time (even if there are no spaces in filename) to prevent any headaches & errors. In this way it is guaranteed that your file will be taken as input properly.<br>

Repeat this command for all the files/folders you copied to the repo.<br>

_Pro tip_ - To stage all new files, folders & subfolders use the following.<br>
`git add -A` _Or_ `git add -all`<br>

#### Commiting the Files

After staging them, check using `git status` to see how many files are being currently being staged.<br>
In my case there's only one file currently staged.
![GitBash Staging Area](/Assets/GB%20Staged%20files.png)

To commit the changes use this command -<br>
`git commit -m "<type a meaningful message here>"`
<br>

For example -<br>
`git commit -m "Added sample file"`
<br><br>
![GitBash Commiting Files](/Assets/GB%20Commit%20Files.png)
<br><br>

### Pushing Commits to Remote Repository

Remote means situated away from local.
In this context, a prime example would be GitHub Repository.

Here I will be using [Demo-repo](https://github.com/MRDGH2821/Demo-Repo).

I have done 2 changes.

1.  Add new file.
2.  Modify existing file.

Here are the commands which I executed.<br><br>
![Demo-Repo part 1](/Assets/GB%20Demo%20repo%20p1.png)<br><br>
![Demo-Repo part 2](/Assets/GB%20Demo%20repo%20p2.png)

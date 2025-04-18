# AI-startup-website
### This project demonstrates the use of git version control system

## Install git
### Visit [Git Website](https://git-scm.com/downloads) download and install git.

Run `git --version` on the terminal to verifi git installation

![git version](./img/git-version.png)

## Signup or login to [Github](https://github.com)

#### Create a new repository named ai-startup-website

![ai-startup-website-repo](./img/creating-remote--repo.png)

![created ai-startup-repo](./img/created-remote-repo.png)

## Create a folder named 'git-project' on the terminal

#### Run the command `mkdir git-project` to a folder named git-project

![create git-project](./img/create-dir.png)

#### Change directory to the one just created ` cd git-project`

![cd to git-project](./img/cd2git-project.png)

## Clone the ai-startup-website repository

#### On the git-project directory clone the ai-startup-website repo. Run the command `git clone [url from the remote repository]`

![clone remote remote](./img/cloning-repo-2.png)

#### Navigate to the just cloned repository
`cd ai-startup-website`

![to the clonned repo](./img/cdai-startup4part2.png) 

#### Create index.html file
![create index.html](./img/createindexhtmlfile.png)

#### Add content to the index.html file

![addingtohtml](./img/addinghtmlcontent.png)

#### Check if changes have been staged.
`git status`

![check if changes staged](./img/gitstatus1.png)

#### Staged the changes on index.html root file

`git add index.html`

![stage index.html](./img/gitaddindex.png)

#### Confirm changes have been staged.

`git status`

![confirm staged](./img/gitstatus2.png)

#### Files in green color have been staged and ready to be committed to local repo.

#### Commit changes to local repository

`git commit -m"This is my first commit"`

![first commit](./img/first-commit.png)

#### Push the commited changes to main branch remote repo.

`git push origin main`

![pushtoremoterepo](./img/git-push.png)

# Part 2 Simulating Tom and Jerry's Work
---

#### Navigate to the cloned ai-startup-website directory
`cd ai-startup-website`

![cd to ai-starup](./img/cdai-startup4part2.png)

#### Confirm current branch
`git branch`

![current branch](./img/verifybranch4part2.png)

#### Create a new branch 'update-navigation'

`git checkout -b update-navigation`

![create-nav-branch](./img/updatenavbranch.png)

#### Run `git branch` to verify switch to update-navigation branch

![verify-nav](./img/verify-nav-branch.png)

#### Add the content _'This is Tom adding Navigation to the AI-website'_  to the index.html file

![add-nav](./img/this-is-tom.png)

#### Run `git status` to see unstaged files in the update-navigation branch

![see-unstaged-navigation](./img/gitstatus-tom.png)

#### Stage the untracked html file in the update-navigation branch

`git add index.html`

![stage-nav](./img/git-add-index-tom.png)

#### Run `git status` to verify that changes have been staged in the update-navigation branch

![staged-nav](./img/git-status-tom-2.png)

#### Commit Tom's changes to the update-navigation local branch

`git commit -m'Update navigation bar'`

![commit2nav](./img/git-commit-nav-bar.png)

#### Push Tom's branch to remote github repo
`git push origin update-navigation`

![push-tom's](./img/git-push-nav.png)


# Simulate Jerry's contribution to the project

#### Switch back to the main branch

`git checkout main`

![back2main](./img/switch-to-main-jerry.png)

#### Pull the latest changes from the update-navigation branch

`git pull origin update-navigation`

![pull4rmnav](./img/git-pull-nav-jerry.png)

#### Create a branch for Jerry's Work named add-contact-info

`git checkout -b add-contact-info`

![add-contact](./img/create-add-contact-branch.png)

#### Open the index.html file and add contact info

```html
<form action="#" method="POST" class="formcarry-form">
        <label for="name">Your Name</label>
        <input type="text" id="name" name="fullName" required />
        <label for="email">Your Email Address</label>
        <input type="email" id="email" name="email" required />
        <label for="message">Your Message</label>
        <textarea name="message" id="message" cols="15" rows=""></textarea>
        <button type="submit">Send</button>
</form>
```

#### Stage Jerry's changes
`git add index.html`

![stage-jerry](./img/git-add-index-add-contact-jerry.png)

#### Commit Jerry's changes

`git commit -m'Add contact information'`

![commt-jerry](./img/git-commit-add-contact.png)

#### Push Jerry's branch to github

`git push origin add-contact-info`

![push-jerry](./img/git-push-add-contact-info.png)

## Here is the Github repository showing branches.

![showing-branches](./img/showing-branches.png)


# Part 3 Merging Changes

### Pull Request from github

![open pull request](./img/about2openpull.png)

![creating pull](./img/abt2creatpullrequest.png)

### Pull request created
![PR created](./img/about2merge.png)

### Merge update-navigation to main branch

![merged](./img/mergedupdate-nav.png)

## Updating Jerry's branch with latest changes

### On the terminal use the following command to switch to Jerry's branch

`git checkout add-contact-info`

![switch branch](./img/checkout-pt3contac-info.png)

### Pull the latest changes from main to add-contact-info branch

`git pull origin main`

![pull main](./img/git-pull-origin-pt3.png)

## Finalizing Jerry's Contribution

### Push Jerry's updated branch to Github

![final jerry](./img/git-push-add-contact-info.png)

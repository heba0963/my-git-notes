# my-git-notes
############ installation:
> git config --global user.name "My github Name"
> git config --global user.email "My_Email@gmail.com"

> git config --global core.editor "code --wait"

### setup the ssh:
> ls ~/.ssh

>ssh-keygen -t rsa -b 4096 -c "My_Email@gmail.com"

> clip < ~/.ssh/id_rsa.pub

on github.com: setting -> ssh nad GPG key -> new Key -> add the pub key!

> ssh -T git@github.com


### Starting with SSH
> git init // adds .git folder

### SSH structure:
working directory - Index - HEAD 

> git add // will add changes from working directory to the Index. For tracking changes
> git commit // will add changes from Index to the HEAD.
> git push // will add changes from HEAD to the github
> git remote add origin $ssh_url

### to get all changes from github
> git pull

### Branches - sperates pushes between team.
> git checkout -b $branchname // switch to a branch
> git status // shows what branch, I am on
> git merge store // merge changes from store branch to master branch! do push also changes to repo

### 
Green files are new files, to add them to our repo
> git add newFile.txt
> git add . // to add every new file to repo
> git commit -m "Added New File"

> git diff

> git push // to push all changes to github repo


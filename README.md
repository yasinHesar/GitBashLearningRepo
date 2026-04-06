# GitBashLearningRepo

Git init
git status
git add -A
Git add file.txt
Git commit -m 'V1.0'
ls -ltrh
Git diff -A
Git diff Head
Git diff --staged
Git diff --
Git diff -- file.txt
Git reset file.txt
Git checkout file.txt
Git log
Git rm file.txt
Git branch
Git branch Newbranch
Git checkout Newbranch
Git checkout master
Git checkout Newbranch
Git merge Newbranch
Cat file.txt
Git branch -d Newbranch
git config --global user.name
git config --global user.email
git config --global --list
git config --local --list
git clone https://github.com/yasinHesar/GitBashLearningRepo.git
git show <commit-hash>
git tag
git tag -a v1.0 -m 'This going to be my first v1.0 of the program'
git show v1.0
git tag -l "v*"

# Create first SSH key for yasinHesar
# Create key for yasinHesar
$ ssh-keygen -t ed25519 -C "yasin.esameili@gmail.com" -f ~/.ssh/id_yasinHesar
create config
nano ~/.ssh/config
Enter the following in the config:
$ cat ~/.ssh/config
# Account 1: yasinHesar
Host github.com-yasinHesar
    HostName github.com
    User git
    IdentityFile ~/.ssh/id_yasinHesar

# Account 2: HesarYasin
Host github.com-HesarYasin
    HostName github.com
    User git
    IdentityFile ~/.ssh/id_HesarYasin

cat ~/.ssh/id_HesarYasin.pub

#you need to have a repository in github first then you can push your local to the remote (Github):
#first make an origion in your computer (local):
git remote add origin git@github.com-yasinHesar:yasinHesar/WorkOnPythonExercises.git
#then you can push or pull (-u means you can push whenever you want without writing origin master . just git push is ok after first time.
git push -u origin master 
or
git pull <remote-name> <branch-name>

this shows which remote you work on:
git remote -v
# How to switch between the Github accounts:
$ ssh -T git@github.com-yasinHesar

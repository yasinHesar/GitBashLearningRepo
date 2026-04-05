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

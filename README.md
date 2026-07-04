# Git-most-commands-
git --version              For check version 
mkdir edureka               for create folder
cd <edureka>            Change directory)go to folder  
git init                    for initialize repository in folder git add &lt;filename>.html  
git add <filename>.html                 for adding html file
git diff                                for checking editing or change code
git status                              for check files nname & modified lines
git commit <filename>.html      commit in local repository to push remote rep 
git commit -a                          for commit all to push remote depositry
git branch fix                          For create branch name fix
git branch                              to check branch list
git check out fix                       to enter/switch in fix name branch
git branch -d fix                       to delete branch name fix
git branch -D                           to delete forcefully branch
git check out master                    to enter/switch in master name branch
git commit -a -m changes from fix branch
fit merge fix                           for merge master with fix branch
git mergetool                         if conflict issue created due to merge
:wq                                     for save & exit
git config --global user.name "bhupinder"
git config --global user. email "bhupinder@gmail.com"



               Lec-14  Beginning Steps2 after yum update for commit,push, pull,adding,connecting local repository with central repo
                     https://www.youtube.com/watch?v=JXiJNCtWmcA&list=PLBGx66SQNZ8aPsFDwb79JrS2KQBTIZo10&index=14
   
login in mumbai EC2 instance
ec2-user
sudo su
mkdir mumaigit &                 create one directory & go inside it 
git init
touch myfile       (put some data)
git status                                 show you data of working area
git add .                         help to add code from dir to staging area  
git commit -m "1st commit from mumbai"      for commit 
git status                                  for checking working area
git log                             show userid,date,commit id etc who commit
git show <commit-id>                      show you what code type by use 
git remote add origin <centralgit url>      to add remote repo
git push -u origin master               local repo connect/push to centra rep
(enter username & password)


              steps 3 for second pc or repository for pull & push 

login in singapore Ec2 instance
create one directory & go inside it
git init
git remote add origin <github repo url>
git pull -u origin master
git log
git show <commit-id>
      Now add some code in file
git status
git add .
git commit -m "singapore update1"
git status
git log
git push origin master

                     Below command for ignore files & checking logs

vi .gitignore then press enter then I       for help to ignore or hidden files
*.css
*.java      esc :wq
git add .gitignore
git commit -m "latest update exclude .css"
git status
touch file1.txt file2.txt file4.css file4.java    to create file 
git status                                       as per command 62 to 64 java & css file will not appear in statu & not will commit
git add.
git status                only .txt file addes not .java & .css
gti commit -m "ignore java & css file"      for commit
git log                                for checking commit
git log 1                              for checking last 1 commit
git log --oneline                      for check all commit
git show paste comit id                specific commit id checking
git log --grep "ignore"                 for checking ignore word realted commit


       Lecture 15 Below command for create branch,Merge,checking logs & stash

git merge branch1                 present in master branch then use to merge with branch1
git log --online                   for checking
git merge log                     to verify merge
git push origin master            then press enter it will ask git hub user name & passw for push to central repo
if confliciting file name during merge then entre into file namen & set content as per required save & exit
git status                       for checking status & then need to add & commit again but not require merge again
git add .                        after setting conflict need to add & commit again .
git commit -m "resolve conflict"
git stash                        for sudden emergency work assign you before addin & commit
git stash list                    for list no 0,1,2 etc
git stash apply stash@1 for return from stash to workspace for adding & commit
git stash clear                  to remove from stash if you already add & commit from stash
git reset .                     to clean staging are only
git reset --hard  to clean both staging area & workspace

                  Lec16 How to do git revert, Tag & github clone

The revert comman help you undo an existing commit
It does not delete any data in the process instead rather git creates a new commit with the included files reverted to their prevoius state o, your version control history move forward while the state of your file move backward

git revert
git clean -n                      before remove untrack file will show you list for remove
git clean -f                      romoved forcefully remove untrack file
git tag -a <tagname> -m <message> <commit Id>    for add tagname, meaage iocommit-Id 
git tag                           to see list of tag
git show <tagname>                to see commit id or tag
git clone <url of github repo>    It creates a local repo automatically in linux with the same name as in github account. 
git tag -d <tagname>              to delet tag name           

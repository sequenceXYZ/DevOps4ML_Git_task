## DevOps4ML_Git_task 🚀
### Hands On GIT task.

#### 1. Install Git Bash.
* install git \
https://git-scm.com/downloads 
* check the installed version  
git --version  
* configure Git username and email   
git config --global user.name "John Doe"   
git config --global user.email "john.doe@noreply. com"  
* check if name and e-mail is set   
git config --list   
* change default branch name to "main"   
git config --global init.defaultBranch main 

#### 2. Initialize a new local repository.
* create directory   
mkdir <directory_name>
* initialize git in the repository   
git init

#### 3. Create a README.md file and put a few lines in there using Markdown syntax. Commit changes to master branch.
nano README.md   
git add .   
git commit -m "commit message"   
git status  

#### 4. Create 3 versions of master branch with names feature_a/b/c.
* create branches  
git branch feature_a  
git branch feature_b  
git branch feature_c  
* see list of all the branches and branch you are currently on  
git branch  

#### 5. Make different changes in each branch and commit them.
* repeat the same commands with branches feature_b, feature_c   
git checkout feature_a   
nano <file_name>   
git add .   
git commit -m "commit message"  

#### 6. Merge changes from all feature branches to feature_d branch.
* create and switch to new branch  
git checkout -b feature_d  
* merge feature_a branch into feature_d; repeat with other brances the same  
git merge feature_a   
git branch --merged   
* delete feature_a branch   
git branch -d feature_a  

#### 7. Merge feature_d to master.
* switch to master branch   
git checkout master  
* merge feature_d branch into master   
git merge feature_d   
git branch --merged   
* delete feature_d branch  
git branch -d feature_d  

#### 8. Check if you have all changes in master branch.   
git branch --merged   
git status  

#### 9. Check what was changed and what was added commit by commit. You could play more with branches and code changes in your local repo to be more familiar with the background processes of Git.   
git log   
git log --oneline  

#### 10. Set up a git remote, pointing to your gitlab/github account. Push the changes and make sure they're accessible for the team.
git remote add origin < remote_repository_URL>   
* to check the remote status   
git remote -v  
* push commits to remote repository in GitHub   
git push -u origin main  

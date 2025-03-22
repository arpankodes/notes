## Uploading a new project to github
Create a new repository on Github.  
```
git init
git add .
git commit -m "First commit."
git remote set-url origin git@github.com:arpankodes/<repo-name>.git
git push origin master
```

## Handling multiple git accounts
Source: [Multiple GitHub accounts](https://www.freecodecamp.org/news/manage-multiple-github-accounts-the-ssh-way-2dadc30ccaca/)

### switch between work and personal git
```
ssh-add -D  
ssh-add ~/.ssh/id_rsa_work_akanungo // for work  
ssh-add ~/.ssh/id_rsa  // for personal  
```
### confirming git user
```
git config user.name "User 1"   // Updates git config user name  
git config user.email "user1@mail.com"
```
### cloning repository
personal  
`git clone git@bitbucket.org-work_akanungo:akaungo/repo_name.git`
Using Personal token  
`git remote set-url origin https://<your-token>@github.com/arpankodes/todo-react.git`
### For Locally Existing Repositories  
List the Git remote of the repository,
```
git remote -v
git remote set-url origin git@github.com-worker_user1:worker_user1/repo_name.git
```

## Remove changes from last commit and preserve in local
`git reset --soft HEAD~`

## Ignoring already committed file
Add that file to .gitignore.  
Remove that file using the command    
```
git rm --cached file_name  
git rm -r --cached folder_name // for removing folder
```
Then commit and push to the remote repository

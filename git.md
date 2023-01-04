## Remove changes from last commit and preserve in local

git reset --soft HEAD~

## Handling multiple git accounts

ref- https://www.freecodecamp.org/news/manage-multiple-github-accounts-the-ssh-way-2dadc30ccaca/

### switch between work and personal git
$ ssh-add -D
$ ssh-add ~/.ssh/id_rsa_work_akanungo // for work

$ ssh-add ~/.ssh/id_rsa  // for personal

### confirming git user
git config user.name "User 1"   // Updates git config user name
git config user.email "user1@workMail.com"

### cloning repository
personal
> git clone git@github.com:arpankodes/repo_name.git

git clone git@github.com:RocketChat/Rocket.Chat.git

work
> git clone git@bitbucket.org-work_akanungo:akaungo/repo_name.git

### For Locally Existing Repositories

List the Git remote of the repository,
> git remote -v

> git remote set-url origin git@github.com-worker_user1:worker_user1/repo_name.git

## Ignoring already committed file

need to add that file to .gitignore.
need to remove that file using the command
> git rm --cached file_name
> git rm -r --cached folder_name // for removing folder

Then commit and push to the remote repository

## create gh repo from cli
> gh repo create

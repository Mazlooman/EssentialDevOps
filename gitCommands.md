# Github 
## Install Git 
 Win: Install [Git](https://git-scm.com/downloads/win)  
 Linux:   `sudo apt install git`   
> :memo: **Note:** create Folder `mkdir my-repository && cd my-repository`

## Proxy Git
### proxy setting
git config --global http.proxy  <Address:Port>
git config --global https.proxy  <Address:Port>

### Remove proxy
git config --global --unset http.proxy
git config --global --unset https.proxy

## Connect to Git
### Method 1: Create SSH-keys and config Github
**SSH Keys**  
Create Public and Private Key
`ssh-keygen -t ed25519 -C "mazlooman@gmail.com"`   
```eval  `ssh-agent -s` ```  
`ssh-add .ssh/githubkey `

**Github**   
  Go to github  
    [Settings/SSH and GPG keys/Add new SSH Key](https://github.com/settings/ssh/new)  
  Then, add pubkic ssh key. 
   
### Method 2: Create HTTPS Token and config Github  
**HTTPS Token**   
[Settings/Developer Settings/Generate new Token](https://github.com/settings/tokens)   

## Repository
### Initialize Local Repository
Initialize a local Git repository  
`git init`  
> :memo: **Note:** After this create .git/ directory on current path.   
### Create Remote Repository on GitHub/GitLab  
`git remote add origin  https://github.com/mazlooman/essentiolDevOps.git`
### Change Remote Origin
Set URL   
` git remote set-url origin https://github.com/username/new-repo.git  `
### Check connectivity Github
`git remote -v`
### Remove Remote connectivity Repository 
`git remote remove origin`
## Operations
### Check Status Files and Directory   
`git status `
### Staging Files and folder 
`git add File.txt`
`git add .`
### Commit Tracking Files and Folders
`git commit -m "Commit message"`   
> :memo: **Note:** Staging current tracking files && Commit it     
`git commit -a -m "Commit message"`
### Push Repository to Github/GitLab
`git push -u origin main`
### Clone Repository from GitHub/GitLab
if already exist repository   
`git clone https://github.com/mazlooman/Git --config "http.proxy=http://<Address:Port>"`
### Restore from Remote Repository 
`git restore <file>`   
`git restore .`   
`git reset --hard origin/main`
## Additional Operation
### Ignore files tracking
```
nano .gitignore 
and then add list of files or format 
f.e
debug.log
*.pub
```
then `git add .gitignore`
and afterthat `git commit -m "Add .gitignore file"`

## Logs Operation
### history commits 
`git log`   
`git log --oneline`   

Rendered Output: 

```
$ git log --oneline
4c834bb (HEAD -> main, origin/main) commit files
98df358 second commit
b98cfe3 initial Commit
```




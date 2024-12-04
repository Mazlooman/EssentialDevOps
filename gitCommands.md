# Github 
## Install Git 
 Win: Install [Git](https://git-scm.com/downloads/win)  
 Linux:   `sudo apt install git`   
> :memo: **Note:** create Folder `mkdir my-repository && cd my-repository`

## Proxy Git
### proxy setting
git config --global http.proxy http://141.53.67.240:9090
git config --global https.proxy http://141.53.67.240:9090

### Remove proxy
git config --global --unset http.proxy
git config --global --unset https.proxy

## Connect Git
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
### Staging Files and folder 
`git add File.txt`
### Commit Tracking Files and Folders
`git commit -m "Commit message"`   
> :memo: **Note:** Staging && Commit    
`git commit -a -m "Commit message"`
### Push Repository to Github/GitLab
`git push -u origin main`
### Clone Repository from GitHub/GitLab
if already exist repository   
`git clone https://github.com/mazlooman/Git --config "http.proxy=http://webgateci.med.uni-greifswald.de:9090"`
### Check Status Files and Directory   
`git status `





# Github 
### Install Git 
 Win: Install [Git](https://git-scm.com/downloads/win)  
 Linux:   `sudo apt install git`   
*Note:* create Folder
`mkdir my-repository && cd my-repository`
### Initialize Local Repository
Initialize a local Git repository  
`git init`  
*Note*: After this create .git/ directory on current path.   
### Create Remote Repository on GitHub/GitLab  
`git remote add origin  https://github.com/mazlooman/essentiolDevOps.git`
### Check connictivity Github
`git remote -v`
### Remove Remote Repository 
`git remote remove origin`
### Clone Repository from GitHub/GitLab
if already exist repository   
`git clone https://github.com/mazlooman/Git --config "http.proxy=http://webgateci.med-uni-greifswald.de:9090"`
### Check Status Files and Directory   
`git status `




## Change Remote Origin
Set URL   
` git remote set-url origin https://github.com/username/new-repo.git  `     
Fetch and Push    
`git remote -v`  
Remove and Add again   
`git remote remove origin `  
`git remote add origin git@github.com:User/EssentialDev.git`




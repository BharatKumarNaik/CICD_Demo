### Git Steps 

`git init` <br>
`git remote add origin [url link]` <br>
`git add filename1 filename2 `<br>
`git add . ` (will add all the files) <br>
`git commit -m "message" ` <br>
`git push -u origin branchName` <br>


### Note: <br>
If face some SSL certificate error <br>
<br>
This will provide the ssl certificate       <br>
`git config --global http.sslbackend schannel `  <br>


if above doesnot work then try this out  <br>
<br>
`git config --global http.sslVerify false ` <br>
`git config --global http.sslVerify true `  <br>

---

`git branch [new branch name]   `     --creating branch           <br>
`git checkout newbranch   `           --getting into new branch   <br>
`git add filename`            <br>
`git commit -m "message"  `       <br>
`git push -u origin main `        <br>

---
## Merging sub branch files to main branch
#### Start a new feature   <br>
`git checkout -b new-feature main   ` <br>
#### Edit some files <br>
`git add [file]`<br>
`git commit -m "Start a feature"`<br>
#### Edit some files<br>
`git add [file]`<br>
`git commit -m "Finish a feature" `<br>
#### Merge in the new-feature branch<br>
`git checkout main `<br>
`git merge new-feature `<br>
`git branch -d new-feature `<br>

---
## Move one file from sub branch to main branch
<url> https://www.youtube.com/watch?v=oXZyQZ_RE5k

---

#### Steps for CICD Pipeline in GitHub
1. setting -> developer setting -> personal acess token -> token -> generate token
2. copy the token
3. go to code uploaded repo -> setting -> secrets and variables -> Actions -> add env variable 
4. setting -> general -> action -> set permision to workflow read and write permission(which is below)
5. go to actions -> python workflow -> create new pipeline -> add the yaml file having jobs -> commit it




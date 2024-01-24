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

--------------------------------------------------------------------------------

`git branch [new branch name]   `     --creating branch           <br>
`git checkout newbranch   `           --getting into new branch   <br>
`git add filename`
`git commit -m "message"  `       <br>
`git push -u origin main `        <br>

----------------------------------------------------------------------------------
## Merging sub branch files to main branch
#### Start a new feature   <br>
`git checkout -b new-feature main   ` <br>
#### Edit some files<br>
`git add [file]`<br>
`git commit -m "Start a feature"`<br>
#### Edit some files<br>
`git add [file]`<br>
`git commit -m "Finish a feature" `<br>
#### Merge in the new-feature branch<br>
`git checkout main `<br>
`git merge new-feature `<br>
`git branch -d new-feature `<br>

# gitnote



## Basic
### Working Tree to Staging Area

``` bash
	#to move file to staging Area
	git add <filename> 
	
	#check the differences between Working Tree and Staging Area
	git diff
	
	#disregarded changes 
	git checkhout -- <filename>
```

### Staging Area to Recent Commit
``` bash
	#commit files
	git commit -m '<msg>'

	#show the differences between stagin Area and recent commit
	git diff --staged

	#remove committed files and the file in working tree
	git rm <filename>

	#get recent commit file 
	git reset HEAD <filename>
```

### Restore Commit files that aren't in Working Tree and Stagin Area

``` bash
#check certain file in git log
git log -- <filename>

# restored file to both staging area and working tree
git checkout <commit log number> -- <filename>

# commit the restored file
git commit -m '<msg>'
```

### create subtree
```
	git subtree push --prefix dist origin gh-pages
```


### Branch

``` bash 
# list branches
git branch

# create new branch call feature/test
git branch feature/test

# check which branch you are in 
git status 

# switch to feature/test
git checkout feature/test

# merge feature/test branch to current branch
git merge feature/test

# adding : to delete remote branch
git push origin :feature/branch

# delete local branch
git branch -d feature/branch
```
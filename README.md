# gitnote

### create subtree
`git subtree push --prefix dist origin gh-pages`

### basic git cmd
```
* Working Tree to Staging Area
	1. use `git add <filename>` to move file to staging Area
	2. use `git diff` to check the differences between Working Tree and Staging Area
	3. use `git chekchout -- <filename>` to disregarded changes 

* Staging Area to recent Commit
	1. use `git commit -m '<msg>'` to commit files
	2. use `git diff --staged` to show the differences between stagin Area and recent commit
	3. use `git rm <filename>` to remove committed files and the file in working tree 
	4. use `git reset HEAD <filename>` to get recent commit file 

```
***

```
* Restore Commit files that aren't in working tree and stagin area
	use `git log -- <filename>` to check certain file in git log
	use `git checkout <commit log number> -- <filename>` to restored file to both staging area and working tree
	use `git commit -m '<msg>'` to commit the restored file
```
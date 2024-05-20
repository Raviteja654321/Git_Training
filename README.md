# Git

Git init

```python
git init
```

Git clone

```python
git clone `link`
```

Git add

```python
git add .

adds a change in the working directory to the staging area.
```

Git commit

```python
git commit -m "Message"

create a snapshot of the staged changes along a timeline of a 
Git projects history.
```

Git stash

```python

temporarily shelves (or stashes) changes you've made to your working copy so 
you can work on something else, and then come back and re-apply them later on

git stash   => will stash the changes made to some temporary address and then we 
								perform git fetch
							
```

.gitignore

```python
put the file names that are not requited in this file with name .gitignore

we can also put the names of folders like node_modules
```

Git fetch

```python
git fetch => will fecth from remote directory to the local directory but 
							not working directory
							
git fetch <remote> <branch>  => Same as the above command, but only 
																fetch the specified branch.
```

Git pull 

```python
git pull or git pull origin main => 
1. is combination of git fetch and git merge.
2. to fetch and download content from a remote repository and
	 immediately update the local repository to match that content

```

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/5e772b93-1b52-4c6a-a2ee-5bea5cac0802/249d1052-1975-40b8-a0e2-34b1934cfc58/Untitled.png)

Git push

```python
git push => to upload local repository content to a remote repository

git push origin main => push to remote origin branch from the local main branch
```

Git tag

```python
git tag => A tag is an object referencing a specific commit within the 
					project history
			

git tag v1.4-lw
```

GIt status:

```python
git status => shows the tract of the file / directories.
```

Git branch

```python
git branch => List all of the branches in your repository

git branch <branch> => Create a new branch called ＜branch＞

git branch -d <branch> => Delete the specified branch
```

Git checkout

```python
git checkout <branch> => switches to the branch 
```

Git merge

```python
## Standard way of doing.
# Start a new feature
git checkout -b new-feature main
# Edit some files
git add <file>
git commit -m "Start a feature"
# Edit some files
git add <file>
git commit -m "Finish a feature"
# Merge in the new-feature branch
git checkout main
git merge new-feature
git branch -d new-feature
```

Git revert | GIt reset

```python
git revert <hash_of_commit> => revert the commit with the hash

git reset <hash_of_commit>  => reset the current HEAD to a previous commit,
														 discarding any changes made after that commit.
```

Git rebase | Git rebase -i

```python
git rebase <branch>

```

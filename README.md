1. "git init" -> Powers ur folder to be managed by git, and initialises a new empty repository. It also creates a .git folder that has all the relevant logic to manage versions of your project 

2. "Working area" -> There can be a buch of files that are not correctly handled by git. It means that the changes done or to be done in those files are not manged by git yet. A file which is in working area is considered not in the staging area. When we do 'git status' and we see a bunch of 'untracked file' then these are actually called to be in the working area.

3. "Staging area" -> What all files are going to be part the part of the next version that will create. This staging area is the place where git knows what changes will be done from the last version to the next version .

4. "Repository area" -> This area actually contains the details of all your previous registered version. And the files in this area, git alredy manges them and knows their version history. 

5. 'git add file' -> moves file from working area to staging area.

6. 'git rm --cached <'file'>' -> moves file back from staging area to wroking area to a repository area.

7. 'commit' -> commit is the particular version of the project.It captures the snapshot of the project's staged changes and creates a version out of it.

8. 'git commit' -> registers staging changes to a commit.

9. 'git log' -> list down all the the commits of the repository. To log out of git log prompt, press 'q'.

10. 'git restore <'files'>' -> it removes all the files changes from the staging area to be commited. This can be useful, if we did some dirty piece of code and now no more want it. Instead of deleting every change line by line, we can restore it or you can say restore last clean version of the file.

11. 'git restore --staged <'files'> -> it removes file from changes from staging area to working area.

12. Diff between git rm and git restore
ans: if you want to move the whole file back to the untracked state, then we do git rm, otherwise if we just want the changes to be moved in working area or staging areathen we do git restore

13. 'git diff commit1 commit2' -> gives the difference of all the file changes between two commits

14. 'git commit -m "<'your commit message'>"' -> If we want to avoid opening a text editor like vim/nano to add commit message we can use this following command 

15. 'git remote' -> list down all the remote connections names. 

16. Remote connections -> It helps you to link two git repos for uploading and downloading changes from each otherwise

17. 'git remote add <'name of remote'> <'link of the remote'>' -> this command helps us to add a new link to the remote repo and give a name to it 

18. 'git remote rm <'name of remote'>' -> deletes a remote connection 

19. 'git remote rename <'oldname'> <'newname'> -> renames the remote connection

Note: The name of the remote connection is always used to establish communication between the repos

20. 'git add <'file1'> <'file2'> <'file3'> -> this command will add multiple file changes togethr in the staging area 

21. 'git add .' -> will add all file from working repo to staging area

22. 'git pull <'remote name'> <'branch name'> : downloads latest changes from the branch of the mentioned remote in your local repo.

### RECOMMENDED PRACTICES

-make changes 
-git add <'file'>
-git commit
-git pull
-git push

1. "git init" -> Powers ur folder to be managed by git, and initialises a new empty repository. It also creates a .git folder that has all the relevant logic to manage versions of your project 

2. "Working area" -> There can be a buch of files that are not correctly handled by git. It means that the changes done or to be done in those files are not manged by git yet. A file which is in working area is considered not in the staging area. When we do 'git status' and we see a bunch of 'untracked file' then these are actually called to be in the working area.

3. "Staging area" -> What all files are going to be part the part of the next version that will create. This staging area is the place where git knows what changes will be done from the last version to the next version .

4. "Repository area" -> This area actually contains the details of all your previous registered version. And the files in this area, git alredy manges them and knows their version history. 

5. 'git add file' -> moves file from working area to staging area.

6. 'git rm --cached <file>' -> moves file back from staging area to wroking area to a repository area.

7. 'commit' -> commit is the particular version of the project.It captures the snapshot of the project's staged changes and creates a version out of it.

8. 'git commit' -> registers staging changes to a commit  

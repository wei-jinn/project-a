# project-a
This project is a demonstration of git version control system learning


Just to get you clear about this:

Working directory:
1. Create new folder
2. git init - to initialise a folder as a local working directory
3. git config --global user.name "name" //to set your name
4. git config --global user.email "gmail.com" //to set your email
5. Add new file: author_description

6. Log in to github.com:
6.1. Create new repository
6.2. Add new file: introduction, add some text, commit.

7. Go back to working directory(via editor terminal), commit all  to local git repository.
8. git status - to check the update status of files in the local repository(as compared to working directory). Green files are the files has same version as git repository while red files are the files that are not updated yet(untracked changes) to the git repository yet.
9. git diff - to check exact difference between working directory and local repository.
10. git add .
11. git commit -m "short message about the commit attempt"
12. At this point, if git status returns "working tree clean", then your working directory and local repository is now tally, at the same page.

13. Connect local repository to the remote repository created in step 6.
14. git remote -v : to view all linked remote git repo
15. git remote add repo_name repo_url
16. before pushing anything to remote repository, pull first.
17. git pull repo_name/origin master: pull everything from current remote repository master branch
18. If unsuccessful, execute step 17 by: git pull repo_name --allow-unrelated-histories master
19. git push -u repo_name/origin master

 



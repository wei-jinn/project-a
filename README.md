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
15. git remote add repo_name repo_url (REPO_NAME, BRANCH_NAME ARE ALL CASE SENSITIVE)
16. before pushing anything to remote repository, pull first.
17. git pull repo_name/origin master: pull everything from current remote repository master branch
18. If unsuccessful, execute step 17 by: git pull repo_name --allow-unrelated-histories master
19. git push -u repo_name/origin master

20. Let's create and work on a branch
21. git branch branch_name: create a branch
22. git branch: to check the existing branch list, the active branch(working branch) is the branch with *
23. git checkout branch_name: switch yourself to work on the branch with branch_name, now branch_name is active branch.
24. At this point, branch_name is just a pointer without any content, you make your changes here which would not affect the local repo master(and remote master too.)
25. Your local active branch is now branch_name, let's add and commit this particular batch of changes to local repository branch, by simply just repeating step 10 - 11
26. If step 25 is successful, then we are ready to commit the changes to remote repository.
27. No worries, the branch will be automatically added to remote repository after committing without having you to create a branch at remote site again.
28. Simply just git push repo_name/origin branch_name, you may check the update from github.com, at remote repository branch_name. 
29. At this point, the latest changes you have made since step 24 is now recorded in both local branch_name and remote branch_name but none of the master.
30. You may say, master branch is now left behind. What to do next is to merge the changes from branch_name to master branch.

31. If you want to merge branch to master, switch active branch to master via git checkout first.
32. Reminder: please ensure you commit every changes made in your current branch before you checkout to other branch.




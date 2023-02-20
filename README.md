#### This project is for the Devops bootcamp exercise for 
#### "Version Control" 

EXERCISE 1: Clone and create new repository

Clone git repository, creating a new local copy and
Push it to your own Gitlab remote repository.

git clone https://gitlab.com/devops-bootcamp3/git-project git-project-ku
cd git-project-ku/
git status
rm -rf .git
git init
git add .
git status
git commit -m "Initial git-project-ku"
    created rep https://github.com/EvgeniyKunegin/git-project-ku
git push --set-upstream origin master -  

-----------------------------------------------------------------------------

EXERCISE 2: .gitignore

You see that build folders and editor specific folders are in the repository and decide to ignore it as a best practice.
- Ignore .idea folder, .DS_Store, out and build folders

Createв file .gitignore
	.idea/*
	.DS_Store

Clear cash
	git rm -r --cached .DS_Store

git add .
git commit
git push

-----------------------------------------------------------------------------

EXERCISE 3: Feature branch

Create a feature branch and change following:

- Upgrade the logstash-logback-encoder version to 6.6
- Add image to the index.html file (url: https://www.careeraddict.com/uploads/article/58721/illustration-group-people-team-meeting.jpg)
You are done with the changes. So:

- Check your changes using "git diff" and
- Commit them if everything is correct.
Note: There is a standard in your team to name commits with descriptive text.

- Push your changes to your remote repository.

Changed index.html 
get-diff

     <h1>Team member roles</h1>
-    <!-- add image here  <img src="" width="" /> -->
+    <!-- add image here  <img src="" width="" addad /> -->
        <img src="https://www.careeraddict.com/uploads/article/58721/illustration-group-people-team-meeting.jpg"  width="" />

git add .
git commit -m "Add img to index.html"
git push
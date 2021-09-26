## What is GitHub used for?
It's used to store your code, different files, game assets and overall project stuff.
Keeps track of versioning, which means you can start with a v0.1 of your project, post many more versions up to v1.0 say, and then come back to v0.1 like it's nothing.
Saves whole history of changes with each of the new stuff description, date and differences between new code and old code (or file contents).
Also allows multiple people to work on the same project without code collisions.

## What you will need
- [Git bash](https://git-scm.com/download/win)
- [Github account](https://github.com/signup)
- Most likely Microsoft account (I'd suggest creating a private one and one for your school, if you haven't got one already) [Microsoft Signup](https://signup.live.com/)


## What is repo
Repo is short for repository, which is basically a container for the code or files you want to upload. Dates, files history, changes, descriptions, contributors and settings are all contained inside a repo.

## Creating a repo
Go and [Create repo](https://github.com/new):
- Name it whatever u want
- Choose privacy; public is available for everyone, private requires a link and an invitation. Both are free now.
- Skip creating files like README, .gitignore and a license for now.

## Uploading first files
You've now created a repo. Now to connect it to the local files.
After creating, you will be shown a list of commands. By now, you should have at least one file that you want to upload, could be anything, but I'd suggest some code.
- Open up GitBash, 'cd' into the folder you have your code in (or right click inside of it and open GitBash directly from there).

Type in:
- git init
- git add .
- git commit -m "Description of commit"
- git branch -M main
- git remote add origin (link to your repo, ex. https://github.com/username/repo_name.git)
- git push -u origin main

This should upload the file to the repo. You can now refresh the repo website and the file(s) should appear inside.

## Uploading more files
Uploading more files is simpler than the first time.

Try changing some lines of code inside the file you uploaded.
After that, open up GitBash again if you closed it, and type in:
- git add .
- git commit -m "Description"
- git push

And that's it. You've commited and pushed changes, and it will now show up in the repo's history.
You can refresh the website again and see that the commit message changed. Click on it to show the differences between old code and new code you just commited.

## Couple of words
GitBash will automatically detect git repository if it exists in the folder you're in, so no need to re-init it.
Commits should be short, straightforward with a descriptive, but not long description. For example, instead of commiting "Changed how players move, players have now 150 hp and do more damage" make three separate commits:
- Changed player movement type
- Players health changed from 100 to 150
- Players do more damage, old 50 new 100

This will allow you to quickly find what you're looking for in the history, save other people's problem and will follow the good principles.

Install 'Git lens' VSC extension, it will allow you to commit, push, revert and check commits from inside the editor without typing in commands. Also subtly shows you breaf history of each line edited in file.

## TL;DR
- Create repo wihtout README, .gitignore and license
- Follow instructions
- Make changes
- git add .
- git commit -m "Changes"
- git push

Done.

## Commands cheatsheet
- [git add](https://www.atlassian.com/git/tutorials/saving-changes)
<details>
	<p>
		Adds files to the commit. Use '.' (dot) to add all the files in current folder.
		<br>Example: git add .
	</p>
</details>

- [git commit](https://www.atlassian.com/git/tutorials/saving-changes/git-commit)
<details>
	<p>
		Commits added files (prepares them to be sent).
		<br>Example: git commit -m "Description"
	</p>
</details>

- [git push](https://www.atlassian.com/git/tutorials/syncing/git-push)
<details>
	<p>
		Sends commited files to repo. This will make the changes appear on the repo website and save them properly.
		<br>Example: git push
	</p>
</details>

- [git branch](https://www.atlassian.com/git/tutorials/using-branches)
<details>
	<p>
		Switches current branch. Allows you to work on different feature or version.
		<br>Example: git branch features
	</p>
</details>

- [git status](https://www.atlassian.com/git/tutorials/inspecting-a-repository)
<details>
	<p>
		Shows current status; commited files, added files, removed files, changed files etc.
		<br>Example: git status
	</p>
</details>
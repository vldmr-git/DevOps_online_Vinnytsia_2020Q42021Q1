# readme.md
### Task1.1 - Git

1. Installed GIT to Ubuntu 20.04.1
2. Changed global configs.  
	terminal commands:

		$ git config --global user.name "vldmr"
		$ git config --global user.email vmstangrit@gmail.com

3. Created account [**vldmr-git**](https://github.com/vldmr-git) on [GitHub](https://github.com)
4. Created repo [**DevOps_online_Vinnytsia_2020Q42021Q1**](https://github.com/vldmr-git/DevOps_online_Vinnytsia_2020Q42021Q1)
5. Created structure  

		m1/  
			task1.1  

6. Cloned repo to my workstation.  
	terminal commands:  

		$ git clone https://github.com/vldmr-git/DevOps_online_Vinnytsia_2020Q42021Q1.git

7. Opened git console
8. Moved to folder task1.1.  
	terminal commands:  

		$ cd m1/task1.1

9. Created empty readme.txt file  
	terminal commands:  

		$ vi readme.txt
		$ git add readme.txt

10. Was made init commit.  
	terminal commands:  

		$ git commit -m "main commit 1"

11. Created **develop** branch and checkouted on it.  
	terminal commands:  

		$ git branch develop
		$ git checkout develop

12. Created empty *index.html* file. Commited.  
	terminal commands:  

		$ vi index.html
		$ git add index.html
		$ git commit -m "develop commit 1"

13. Created **images** branch and checkouted on it. Added images folder with images inside it. Not Commited.  
	terminal commands:  

		$ git branch images
		$ git checkout images
		$ cp -r ~/img ~/DevOps_online_Vinnytsia_2020Q42021Q1/m1/task1.1
		$ git add img/

14. Changed *index.html*. Added images source inside it. Commited.  
	terminal commands:  

		$ vi index.html  

	code:  

		<html> 
			<body>
				<img src="img/1111.png">
				<img src="img/2222.png">
				<img src="img/3333.png">
			</body>
		</html>  

	terminal commands:

		$ git add index.html
		$ git commit -m "images commit 1"

15. Returned to **develop** branch  
	terminal commands:  

		$ git checkout develop

16. Created **styles** branch and checkouted on it. Added styles folder with styles source inside it. Commited.  
	terminal commands:  

		$ git branch styles
		$ git checkout styles
		$ cp -r ~/styles ~/DevOps_online_Vinnytsia_2020Q42021Q1/m1/task1.1
		$ git add styles/
		$ git commit -m "styles commit 1"

17. Changed *index.html*. Commited.  
	terminal commands:  

		$ vi index.html  

	code:  

		<!DOCTYPE html>
		<html>
			<head>
				<link rel="stylesheet" href="styles/styles.css">
			</head>
			<body>
				<h1>This is a heading</h1>
				<p>This is a paragraph.</p>
			</body>
		</html>  

	terminal commands:  

		$ git add index.html
		$ git commit -m "styles commit 2"

18. Returned to **develop** branch.  
	terminal commands:  

		$ git checkout develop

19. Merged branches **images** and **styles** into **develop**  
	terminal commands:  

		$ git checkout develop
		$ git merge images  

	cuted terminal message

	> Updating 0149fce..0ab3e1b
	> Fast-forward  

	terminal commands:  

		$ git merge styles  

	cuted terminal message:  

	> Auto-merging m1/task1.1/index.html
	> CONFLICT (content): Merge conflict in m1/task1.1/index.html
	> Automatic merge failed; fix conflicts and then commit the result.  

	terminal commands:  

		vi index.html  

	code:  

		<!DOCTYPE html>
		<html>
			<head>
				<link rel="stylesheet" href="styles/styles.css">
			</head>
			<body>
				<h1>This is a heading</h1>
				<p>This is a paragraph.</p>
				<img src="img/1111.png">
				<img src="img/2222.png">
				<img src="img/3333.png">
			</body>
		</html>  

	terminal commands:  

		$ git add index.html
		$ git commit -m "develop commit 2 after merge images and styles and resolve conflict"

20. Branches were not deleted
21. Merged **develop** into **main**  
	terminal commands:  

		$ git checkout main
		$ git merge develop  

	cuted terminal message:  

	> Updating ab6ee58..46cfcfe
	> Fast-forward  

22. Called `git log` command. Viewed options of `git log` command
23. Pushed all my changes with all branches to origin.  
	terminal commands:  

		$ git push origin --all  

	terminal message:  

	> Username for 'https://github.com': vldmr-git  
	> Password for 'https://vldmr-git@github.com':  
	> Enumerating objects: 40, done.  
	> Counting objects: 100% (40/40), done.  
	> Compressing objects: 100% (29/29), done.  
	> Writing objects: 100% (37/37), 368.58 KiB | 4.09 MiB/s, done.  
	> Total 37 (delta 9), reused 0 (delta 0)  
	> remote: Resolving deltas: 100% (9/9), completed with 1 local object.  
	> To https://github.com/vldmr-git/DevOps_online_Vinnytsia_2020Q42021Q1.git  
	>    6371306..46cfcfe  main -> main  
	>  * [new branch]      develop -> develop  
	>  * [new branch]      images -> images  
	>  * [new branch]      styles -> styles  

24. Executed command `git reflog` and saved it content to */home/vldmr/task1.1_GIT.txt*
25. Added my trainers to repository as collaborators:  

![collaborators](/m1/task1.1/readme_md/collaborators.png)

26. Added *task1.1_GIT.txt* to my local repo and pushed it in GitHub repo.
27. Made file *readme.md* in folder *task1.1* and described results of my work with Git  
28. Described what is DevOps
29.
	> Devops is about deployment and maintenance of infrastructures in software production process 
	> thats why engineers require to navigate a lot of corresponding technologies 
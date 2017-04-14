This page has been contributed by @kch5559

**GitHub** is an online project hosting service that uses Git as its versioning system. You will be assigned into private repositories that will contain homework assignments.

##Contents

* [Setting up **Git**](#setting-git)  
* [How to generate a SSH key](#generating-ssh)  
* [Using **GitHub** for homework](#github-for-homework)  
* [Additional Resourses about **Git** and **GitHub**](#additional-resources)  


## <a name="setting-git"></a>Setting up Git

1. Download Git from the following link:  
[Git - Download](https://git-scm.com/downloads)
2. Open the terminal application.
	* *Window*
		1. `WinKey` + `R`
		2. Input `cmd`
		3. `Enter`
	* *Linux*
		- `Ctrl` + `Alt` + `t`
	* *Mac*		
	   1. Open `Spotlight`  
	   *The magnifying glass icon in the upper-right corner of the menu bar*
	   2. Type `terminal`
	   3. `Enter`
	   
3. Type the following commands on terminal.  
**"YOUR NAME" should be your first and last name.** 
	```$
	git config --global user.name "YOUR NAME"
	```  
**"YOUR EMAIL ADDRESS" should be your email address.**
	```$
	git config --global user.email "YOUR EMAIL ADDRESS"
	```

## <a name="generating-ssh"></a>Generating a SSH key
1. Checking for existing SSH keys:  
 ***if you have an existing key you can skip to step 3 and use it on your github account***  
  <https://help.github.com/articles/checking-for-existing-ssh-keys/#platform-linux>  
2. Generating a new SSH key:  
<https://help.github.com/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent/>
3. Adding the new SSH key to GitHub account:  
<https://help.github.com/articles/adding-a-new-ssh-key-to-your-github-account/>

##<a name="github-for-homework"></a>Using GitHub for Homework
#### Fork a repository
Forking lets you create a copy of a repository under your account. This way you can modify your fork without changing the original repository.  

Click `Fork` button to create a copy of the repository under your account.  


![Github-Fork](https://raw.githubusercontent.com/csc340-03-fall-2016/Image/master/github-fork.png?token=AKzNSvz0qrOhmmAyNJjbaANj16qms6Aqks5XyK0jwA%3D%3D)

#### Clone a repository
Clone checks out the repository on your local computer. 

1. Open your forked repository.  
2. Click Clone or download button on upper-right side and copy either SSH or HTTPS.   
 
   
	![Github-Clone](https://raw.githubusercontent.com/csc340-03-fall-2016/Image/master/github-clone.png?token=AKzNSt4uHL_SIb87GCPeiU0O4mX9H-YEks5XyhzCwA%3D%3D)  
	>//todo change hwX.git -> official hw format  
	>SSH form -  ***git@github.com:your-account-name/hwX.git***   
	>HTTPS form - ***https://github.com/your-account-name/hwX.git*** 

	  
3. Open terminal and type the following command.  
***[SSH or HTTPS] should be replaced for your copied SSH or HTTPS***  
	```$
	git clone [SSH or HTTPS]
	```  
4. By default git clone checks out the `master` branch.

#### Commit
Commits are unit of changes in git. 

* Change your working directory to the cloned directory.  
 e.g. If you clone a repository called foo, cloning creates a directory called 'foo'.  
	```$
	cd foo
	```
* `git add` adds new files for commiting. `--all` adds all files that are not tracked.  
	```$
	git add --all
	```  
If you want to add a specified file you can type the file path instead of `--all`.   
 e.g. If you want to add a cpp file called 'HelloWorld.cpp'.   
	```$
	git add foo/HelloWorld.cpp
	```
* Commit your change with your commit message - e.g Initial commit.  
	```$
	git commit -m "commit message"
	```
*  Update the remote repository.  
	```$
	git push
	```

#### Pull Request
Pull requests allow to tell others about your changes that you've pushed to a repository.   
You **MUST** make pull request when you are fully done with an assginment.
   
1. Make a pull reqeust on your assignment repository.  
![github-pull-request](https://raw.githubusercontent.com/csc340-03-fall-2016/Image/master/github-pull-requests.png?token=AKzNSuWHdDuutQAPsZA2gUkU8PAxr5Tlks5Xv4kjwA%3D%3D)
2. Click `pull request` button.





## <a name="additional-resources"></a>More Resources about Git and GitHub

* Learn about GitHub from this video:
<https://www.udacity.com/wiki/ud775/install-git>

* 15 minutes Git Tutorial: <https://try.github.io/levels/1/challenges/1>

* Additional resources:
<https://en.wikipedia.org/wiki/Git_(software)>




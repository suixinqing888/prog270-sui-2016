# Create your Git folder
##Do this in your  ~/Git folder:
```
mkdir prog270-lastname-2016
cd prog270-lastname-2016
git init
git remote add origin git@github.com:<ACCOUTNAME>/<REPONAME.git>
```
### Example:
	git remote add origin git@github.org:charliecalvert/prog270-lastname-2016.git

## Init your Git folder
```
Do this in your  ~/Git folder:
mkdir prog270-lastname-2016
cd prog270-lastname-2016
git init
git remote add origin git@bitbucket.org:<ACCOUTNAME>/<REPONAME.git>
```
### Example:
	git remote add origin git@bitbucket.org:username/prog270-lastname-2016.git

## Add some content

 you can use the following commands to  add some content to your repositery

```
echo node_modules >> .gitignore
echo .metadata >> .gitignore
echo .idea >> .gitignore
echo bower_components >> .gitignore
echo components >> .gitignore
echo Thumbs.db >> .gitignore
echo *.zip >> .gitignore
```
## Git commit command

```
git add README.md
git add .gitignore
git commit -m 'Initial commit
git push -u origin master
```

## Sample code from GitHub
### Create new respository from command line:
```
echo "# prog270-calvert-2016" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin git@github.com:charliecalvert/prog270-calvert-2016.git
git push -u origin master
```
### Push existing repository from command line:
```
git remote add origin git@github.com:charliecalvert/prog270-calvert-2016.git
git push -u origin master
```
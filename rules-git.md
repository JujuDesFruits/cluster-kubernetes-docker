# 1
Everthing should be in english, doesn't matter what's your level

# 2
When you commit, think to give a description with the title

# 3
Never work on the master branch

# 4
Enjoy



### Here is tips to use git:
* get repository in your folder:
```
git clone https://github.com/JujuDesFruits/cluster-database-docker.git
```
or use ssh to disable password identification (think to add our rsa key)
```
git clone git@github.com:JujuDesFruits/cluster-database-docker.git
```
* work with your branch
```
git pull
git checkout -b name_of_your_branch
```
then you can work
```
git pull
git commit -a
git checkout master
git merge name_of_your_branch
```

* publish a version of the work
```
git tag name_of_your_tag
```

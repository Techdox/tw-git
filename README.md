# Team Workshop: GIT
This workshop is setup to help understand the basics of GIT and how to get up and running using it.

## Cloning a Repo
Cloning a Repo can be completed a couple of ways, such as HTTPS or SSH. 

If you are cloning a repo via HTTPS then you will need to enter in your credentials. Otherwise is you choose to use SSH, you will need to have your SSH key uploaded into your Github.

```
git clone {repo address}
```

## Making changes and commiting those changes
When you have cloned a repo you then will need to commit and push those changes so they are reflected in the repo.

This command will add all changes, otherwise you can remove the "." and name the files you wish to push.
```
$ git add .
```
This command will attach a commit message to your changes so they can be tracked.
```
$ git commit -m "commit message here"
```
This command will push your changes to your repo.
```
$ git push
```

## Master Branch vs Other branches
For best practice, all development should be done on a branch other than Master, such as a branch called Dev. Once the changes on Dev have been made and tested, the changes get reviewed and approved for merge into the Master branch.

```
$ git checkout -b {branch name}
```
The above is shorthand for

```
$ git branch dev
$ git checkout dev
```

## Merging branches
Merging branches is when you merge the code from a branch for example named dev to another one, say the Master branch. When you want to merge branches you typically create what's called a Pull Request. 

A Pull Request is when you specify that you want to merge two branches and you typically select a couple of users to check your request, and then that is approved and merged, normally via the Github console.

If you want to run a merge directly via the console, follow the below commands.

```
$ git checkout master
```
```
$ git merge dev
```


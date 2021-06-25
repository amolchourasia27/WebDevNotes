# Connecting git and GitHub

Before Going furthure we will learn come basics command of cli or command line interface

---

1.``cd`` command to change the directory from current folder 



1.``ls`` command to print all the files and folder of working directory



1.``pwd`` command to print the directory we are working on


---
Now basic are over

## Lets continue 

How `cd` command works is we write `cd` and then we write the folder name

After that we move to our git folder using cd command

Then we will cross check our Working directory by using `pwd`



## Now its time to connect Github to git 

``` git config --global user.name "Your_github_Username"```

aftre that 

``` git config --global user.email Your_github_email```


next commmand is ```git clone``` and we will add repo address after the command

What git clone does that it creates the clone of repo locally in your device 


## Modifying changes

now we have a clone of our repo we can modify chang or create new file in this cloned repo or local folder

```git status``` we can see what change we applyed in our local folder

now we will use ```git add``` to add files in staging area 

after that we will ```git commit -m``` to commit these changes 


now its time to push the changes in online repo using ```git push -u origin main```


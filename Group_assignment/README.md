# Group assignment
To complete the following assignment you need to work in groups, preferrably pairs  
In the following sections we'll note if an action is to be performed individually or as a group.

## First get a local copy (individually)
Begin by clicking the **Fork** button in the header of the repository    
After Forking is complete, click the **Clone** button, copy the url for either HTTPS or SSH  
In GitBash, navigate to the directory where you keep all your git repos by entering the following command:
```cd ~\Documents\git```  
Once in the git directory, clone the repo by entering ```git clone <paste url here>```, you now have a local copy

## The assignment
### Start making changes
Each group should be editing their own file, align beforehand which group will edit which file.  
```Individually``` - Once the file your group will work on has been chosen, open that file in a text editor and edit the python code as instructed inside the file  
Save the file and return to you git terminal, enter ```git status``` and observe the output. Git tells you what it thinks you should do next!


### Commit & push your changes
```Group``` - commit the changes of **one** of the group members
```bash
git add .
git status # read the status message
git commit -m "added print statement by <your name here>"
git status
git push
git  status
```
As you can see, ```git status``` is a very useful command.


### Make a pull request
```Group``` - Have the person who's changes got pushed go to their forked repository.
Right below the **Clone or download button** you should see the link for **Pull request**, click it.
Pull requests are used to merge changes from a forked repository back into the original. 
Before the original owner accepts your request he often reviews your code for code quality and bugs. 
So make sure your code is clean and it's clear how your additions benefit the original code!
The instructor will now accept your request. Repeat the above steps for the other groupmembers.

### Solve merge conflicts
```Group``` - When creating the Pull request of the next groupmember you will run into a merge conflict.
The code on GitHub has already been updated with the changes of the other groupmember!  
Under your repository name click **Pull requests**, click on the request with a merge conflict that you'd like to resolve.  
Near the bottom of the Pull request click **Resolve conflicts**  
Edit the file to keep your changes, the other changes or both and remove the conflict markers (<<<<, =====, >>>>>)
Once the merge conflicts are resolved click **Mark as resolved** in the top right. 
Next click **Commit merge**, review your commit and click **I understand, update BRANCH**. 
Well done! The Pull-request can now be merged.

## Sources used
[How to Fork a repo](https://help.github.com/en/articles/fork-a-repo)  
[How to solve merge conlficts](https://help.github.com/en/articles/resolving-a-merge-conflict-on-github)
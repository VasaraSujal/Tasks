##### Task 1: Install and Configure Git

1. Configure Git with your username and email:
```
  git config --global user.name "Your Name"
  git config --global user.email "your-email@example.com"
```

2. Use git config --list to verify your configuration.
```
   git config --list
```

##### Task 2: Initialize a Repository

1. first of all create a new folder on desktop
```
     mkdir new_folder
```
2. navigate to that folder
```
    cd new_folder
```
3. Initialize git 
```
    git init
```


#### Task 3: Create a File and Make Multiple Commits

1. Create a new file in this folder with echo command
```
    echo "new_file" >> new_file.txt
```
2. Add this file to the stagging area
```
    git add new_file
```
3. Add commit to the file
```
    git commit -m "New commit"
```
4. Make the change to this file
```
    echo "make changes" >> new_file.txt
```
5. add the file to stagging area
```
    git add new_file
```
6. Make commit to this file
```
    git commit -m "Updated text"
```

#### Task 4: Check Status and Log

1. To check the status of current repository using status command
```
    git status 
```
2. view the commit history
```
    git log
```

#### Task 5: Create and Clone a Repository

1. First create a new repository on GitHub

2. Then clone the repository in your local device
```
    git clone (url)
```

#### Task 6: Understanding the Git Workflow

1. Create file in working directory
```
    echo "workflow" >> workflow.md
```
2. Add the file into stagging area
```
    git add workflow.md
```
3. Add commit to this file
```
    git commit -m "Commit added"
```

#### Task 7: Branching and Merging

1. Create a new branch named branch1
```
    git branch branch1
```
2. Navigate to this new branch we use checkout/switch command
```
    git checkout branch1
```
3. Make a new file in the working directory
```
    echo "index" >> index.html
```
4. Add the file to stagging area
```
    git add index.html
```
5. Add commit
```
    git commit -m "Added index"
```
6. To merge branch1 to main branch first we switch to the main branch
```
    git checkout main
    git merge branch1
```

#### **Task 8: Handling Merge Conflicts**

1. Create two branches named branch-A and branch-B
```
    git branch branch-A
    git branch branch-B
```
2. To merge branch-A to main we switch to main branch
```
    git checkout main
    git merge branch-A
```
3. Then we merge branch-B
```
    git merge branch-B
```
4. Resolve the conflict menually
```
    git add README.md
    git commit -m "Resolved merge conflict"
```

#### Task 9: Renaming and Deleting Branches

1. to Rename the branch use branch -m
```
    git branch -m branch-A new_branch
```
2. To delete the file
```
    git branch -d branch-B
```

#### Task 10: Using Git Stash


1. We changes to the file but do not use commit then we use stash to save the changes temporary
```
    echo "Temporary work" >> temp.md
```
2. git stash is used to save the current working directory
```
    git stash
```
3. To view stashed changes we used stash list
```
    git stash list
```
4. To apply the stashed changes use stash apply
```
    git stash apply
```
5. To drop the stash after applying use Stash drop  
```   
   git stash drop
```

#### Task 11: Rewriting History with Interactive Rebase

1. Create multiple commits:  
```   
    echo "Commit 1" > file1.txt && git add file1.txt && git commit -m "Commit 1"
    echo "Commit 2" > file2.txt && git add file2.txt && git commit -m "Commit 2"
    echo "Commit 3" > file3.txt && git add file3.txt && git commit -m "Commit 3"
```   
2. To take the third commit in  top
```
    git rebase -i HEAD~3
```

#### Task 12: Cherry-Picking Commits

1. Apply a specific commit to another branch:  

   This command takes a specific commit from another branch and applies it in current branch. It means that it is copy text from another branch without merging it

```
   git cherry-pick <commit-hash>
```

#### Task 13: Tagging Commits

1. Create and add a tag
```
   git tag -a v1.0 -m "Version 1.0 release"
```
2. Push tag in your repository
```
   git push origin v1.0
```

#### Task 14: Working with Remote Repositories

1. Add a remote repository in your github
```
    git remote add origin "url"
```
2. Push the changes to the remote repository
```
    git push origin main
```

#### Task 15: Forking and Contributing
1. Fork a repository on GitHub.  

2. Clone the fork repository in your local device   
```
   git clone "repo url"
```

3. Open a pull request

#### Task 16: Simulate Team Collaboration

1. Create a repository and share it with a friend.  
2. Both make changes to the same file simultaneously.  
3. Practice resolving merge conflicts and pushing changes.

#### Task 17: Git Ignore

1. Create a gitignore file:  
```
   echo "node_modules/" > .gitignore
```
2. Add files and confirm that ignored files are not staged:  
```
   git add .
```
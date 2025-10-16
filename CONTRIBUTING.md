# Steps for submitting pull requests, coding standards, etc.

### In order to **push** your changes to a branch on the main repository, you will need to make a **Pull Request**!

In case you don't know what a Pull Request (PR) is, it is how teams contribute code changes to projects.

PR's allow others to review your work, suggest improvements, and make sure everything is consistent **before merging** into the main branch.

# How to Submit a Pull Request (PR)

Pull Requests (PRs) are how we contribute code changes to this project.  
They let others review, test, and approve updates before merging them into the main branch.

Follow these steps below whenever you make updates to the codebase!

# Syncing Forked Repository and Main Repository:
Head to the bottom of this page to learn how to sync your forked repo to see main repo's latest changes!

---

## Step 1: Fork the Repository

Because we will be having many people work on this in different parts, each person/group will be working on a **forked** version of the repository. Which is basically making a copy of the repository and you will be able to edit it locally. Once you make your changes, you can then push them to your fork and then request a Pull Request to submit your changes. 


**Making a new branch in your forked repository:**
- Sometimes you will need to create separate branches in order to separate your work. Follow the command and instructions below to make one if you aren't going to be working on main!
bash
```git checkout -b your-branch-name```

- Tip: Use descriptive branch names, such as:
  - fix/image-upload-bug
  - feature/add-login-page
  - docs/update-readme

## Step 2: Push Your Branch to Main (if new branch)

- Same with pushing your changes to a branch, you also have to **push** your branch to main
- bash: ```git push origin your-branch-name```

## Step 3: Make Your Changes

Edit the files in your branch.
Keep your code clean, readable, and well-documented!

## Step 4: Test Your Code

Before pushing, make sure your code:
  - Runs without errors
  - Doesn’t break existing functionality

## Step 5: Add and Commit Your Changes

Once your edits are ready, stage and commit them:

**Stage:** ```git add .``` 
- Before making any commits, you must **stage** your changes which basically lets Git know which changes you actually want to 'save'/commit

**Commit:** ```git commit -m "Add short, clear message describing your changes"```

Example:
```git commit -m "Added image compression function for uploads```

## Step 6: Create a Pull Request

- Go to your **forked** repository on GitHub.
- Click “Compare & pull request.”
- In the PR form:
  - Confirm the base repository is the original project (CareTechUCI/general-project-fall25.git)
  - Confirm the head repository is your fork (yourusername/yourforkedrepositoryname)
  - Add a short title and description of your changes.
- Click “Create Pull Request.”
- Tag your reviewer (e.g., @TechLead, @President).
- If you think it is necessary, you can also add photos as well!

## Step 7: Code Review

- Someone will review your PR.
- They might request small changes but don’t worry, this is part of the process!

Once approved, your PR will be merged into the main branch :D 🥳


## Syncing Your Forked Repository with Main Repository
So what happens if the main repository has new changes but your forked repository was made a week ago and you would like to add these new changes? 

**Do you have to make a new forked repository?** (Thankfully) No!

The way open-source projects work is that each person/group has to work on a forked repository, makes PRs, and then every now and then **syncs** their
forked repository with the main one. 

**Sync** your forked repository to the main repository by running these commands:

1. Add the main CareTech repo as an “upstream” remote (only needs to be done once):

```git remote add upstream https://github.com/CareTech-General/general-project-fall25.git```


3. Fetch the latest updates from the main repo:
```git fetch upstream```


4. Switch to your local main branch:
```git checkout main```


5. Merge the updates from upstream into your main:
```git merge upstream/main```


6. Push those synced changes to your fork on GitHub:
```git push origin main```

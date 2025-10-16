# Steps for submitting pull requests, coding standards, etc.

### In order to **push** your changes to a branch, you will need to make a **Pull Request**!

In case you don't know what a Pull Request (PR) is, it is how teams contribute code changes to projects.

PR's allow others to review your work, suggest improvements, and make sure everything is consistent **before merging** into the main branch.

# How to Submit a Pull Request (PR)

Pull Requests (PRs) are how we contribute code changes to this project.  
They let others review, test, and approve updates before merging them into the main branch.

Follow these steps below whenever you make updates to the codebase!

---

## Step 1: Create a New Branch

Before making changes, create a new branch so you don’t directly edit the main branch. If you have a branch you are working on already, you can skip this step!

bash
```git checkout -b your-branch-name```

- Tip: Use descriptive branch names, such as:
  - fix/image-upload-bug
  - feature/add-login-page
  - docs/update-readme

## Step 2: Make Your Changes

Edit the files in your branch.
Keep your code clean, readable, and well-documented!

## Step 3: Test Your Code

Before pushing, make sure your code:
  - Runs without errors
  - Doesn’t break existing functionality

## Step 4: Add and Commit Your Changes

Once your edits are ready, stage and commit them:

**Stage:** ```git add .``` 
- Before making any commits, you must **stage** your changes which basically lets Git know which changes you actually want to 'save'/commit

**Commit:** ```git commit -m "Add short, clear message describing your changes"```

Example:
```git commit -m "Added image compression function for uploads```

## Step 5: Push Your Branch to Main

- Same with pushing your changes to a branch, you also have to **push** your branch to main
- bash: ```git push origin your-branch-name```

## Step 6: Create a Pull Request

- Go to the repository on GitHub.
- Click “Compare & pull request.”
- Add a title and a description explaining your changes.
- Tag your reviewer (e.g., @TechLead, @President).
- Click “Create Pull Request.”
- If you think it is necessary, you can also add photos as well!

## Step 7: Code Review

- Someone will review your PR.
- They might request small changes but don’t worry, this is part of the process!

Once approved, your PR will be merged into the main branch :D 🥳

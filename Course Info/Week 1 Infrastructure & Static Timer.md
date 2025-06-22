# Week 1: Infrastructure & Static Timer

### Create `earlyexit.fun` GitHub repo

#### create a new repository on the command line

```bash
echo "# earlyexit.fun" >> README.md    //Create a README.MD file
git init      //Initiate git on the folder
git add README.md   //Stage the README.md 
git commit -m "first commit"  //Commit the README.md
git branch -M main            //Stage the maim branch
git remote add origin https://github.com/sheepnir/earlyexit.fun.git //Set the origin folder to a remote repo 
git push -u origin main  //Push the code
```



### Git Workflow

1. Start from main and pull latest changes

```bash
git checkout main
git pull origin main
```

2. Create a new feature branch

```bash
# Use descriptive branch names like: feature/countdown-timer, fix/auth-bug, etc.
git checkout -b feature/static-countdown
```

3. Do your development work

```bash
# Make your changes in Cursor
# Test your changes
```

4. Stage and commit your changes

```bash
git add .
git commit -m "Add static countdown timer to retirement date"
```

5. Push your branch to GitHub

```bash
git push -u origin feature/static-countdown
```

6. Create a Pull Request

- Go to your GitHub repository
- You'll see a yellow banner asking if you want to create a PR
- Click "Compare & pull request"
- Add a description of what you built
- Click "Create pull request"

7. Review and merge

- Since you're working solo, you can merge immediately
- Click "Merge pull request" → "Confirm merge"
- Delete the branch after merging

8. Clean up locally

```bash
# Switch back to main
git checkout main

# Pull the merged changes
git pull origin main

# Delete the local feature branch
git branch -d feature/static-countdown
```

###  Practice the Workflow

Let's practice this workflow by making a small change:

```bash
# Make sure you're on main
git checkout main

# Create a practice branch
git checkout -b feature/update-readme

# In Cursor, add this line to your README.md under "Development Setup":
# ```
# ## Week 1 Progress
# - [x] GitHub repository created
# - [x] Git workflow established
# - [ ] Static countdown timer
# - [ ] AWS Amplify setup
# ```

# Stage and commit
git add .
git commit -m "Update README with Week 1 progress tracking"

# Push to GitHub
git push -u origin feature/update-readme
```

Now go to GitHub and create your first PR!

### Quick Reference: Git Commands You'll Use Daily

bash

```bash
# Check status
git status

# See what branch you're on
git branch

# Switch branches
git checkout branch-name

# Create and switch to new branch
git checkout -b new-branch-name

# Stage all changes
git add .

# Commit with message
git commit -m "Your commit message"

# Push to GitHub
git push origin branch-name

# Pull latest changes
git pull origin main
```

### Next Steps

Once you've completed this setup and practiced the workflow:

1. **Verify everything works**: You should have your repo on GitHub with README and .gitignore
2. **Practice the workflow**: Create that practice branch and PR
3. **Get comfortable with Cursor**: Make sure you can edit files and use the terminal

Ready for the next step? We'll create the static HTML countdown timer and start setting up AWS Amplify. Let me know when you've completed these steps and want to move on to building the actual countdown timer!
# Tech365 Team Collaboration Project on Git and Github

This repository is for a simple Github collaboration exercise.

## Task Overview

Each team member will:

1. Clone this repository "https://github.com/agbatakenneth/tech365-teamProject.git".
 
2. Create a new branch with their name.
   
3. Add their name to the "document.txt" file on a new line.
 
4. Commit and push their changes.
 
5. Create a "Pull Request" for review and merging into the main branch
    

## Step 1: To be taken by the repository owner.

1.1 Create the Github repository

1. Log into your Github account,
 
2. Click on the "+" icon in top right corner --> and select "New repository"
 
3. Fill in the repository details: eg. Repository name: tech365-teamProject, leave it at public, and click "Create repository" at the bottom.

1.2 Go to your git bash terminal and run the following codes sequentially:

. # Create and navigate to the project directory wih

. mkdir tech265-teamProject

. cd tech365-team_project

. # Create document.txt with initial content

. echo "Team Members:" > document.txt

. echo "===================" >> document.txt

. # Initialize the git repository with

. git init

. # Change branch name from "master" to "main" with

. git branch -M main (ignore if your default branch is already "main") 

. # Add remote origin with

. git remote add origin https://github.com/agbatakenneth/tech365-teamProject.git 

. # Stage and commit initial files with

. git add .

. git commit -m "First commit with document.txt

. # Push to main branch with 

. git push -u origin main 


1.3  Configure Branch Protection Rules

. Go to the created repository on Github --> you will see "settings", click on it and select "Branches"

. Under "Branch protection rules", click "Add rule"

. Set: Branch name pattern: main, select "Require pull request reviews before merging, under Approval (select 1) and click "create".

1.4 Add collaborators

. Go to repository --> click on "setting" and then collaborators

. Click "Add people"

. Enter team members Github username or emails

. Send invitations

## Step 2: To be taken by Team members.

. First make sure you go to your email and accept the pending invite before commencing with the under listed procedures

. Go to your git bash and run the following codes sequentially

. # Clone the repository with

. git clone https://github.com/agbatakenneth/tech365-teamProject.git

. cd tech365-teamProject

. # Create and switch to new branch using your name (replace Agbaken with your name)

. git checkout -b agbaken-feature

. # Add your name to the "document.txt" with

. echo "Femi Bello" >> document.txt

. # Commit and push with

. git add document.txt

. git commit -m " Add Femi bello to team member"

. git push -u origin agbaken-feature (replace agbaken-feature with the name you gave to your branch

## Step 3: Create "Pull Request" this action is to be carried out by team members.

. Go to Github, you will see a notification about recently pushed branch

. Click "Compare and pull request" and fill in "Title:" **Type Femi Bello** to team members and then click "Create pull request.

## Step 4: Owner of repository to review and merge

. Go to repository --> Pull request tab

. Open the pending pull request

. Review changes changes in "File changed" tab

. Click "Review changes" --> "Approve"

. Click "Merge pull request"

. Choose merge method (squah merge recommended)

. Click "Confirm merge"

. You can confirm the merge with the code --> git checkout main && git branch --merged | grep branch-name

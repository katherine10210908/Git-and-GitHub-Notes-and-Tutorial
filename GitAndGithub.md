# Git And GitHub

## Repository Creation
### 1. Set up remote GitHub repository 
Do not include README.md for the purpose of this tutorial.
Copy the URL
### 2. Initialization

1. Create folder and file for the project.
2. Command `git init`
2. `git add .` put current work in a staging area
3. `git commit -m ""` - takes a snapshot of the current state of your work 
3. `git branch -M main ` rename your main branch (default name was master)
4. Connect to remote repository  ` git removce add https:// ... git` your copied url
5. `git push -u origin main` push the main branch to remote repository 
-u -> 它会让 Git 记住这次的对应关系。

## Branching and Merging 
!! Never edit or write on main. 
Main -> production 
### 1. Create and switch to a branch 
`git switch -c add-new-chapter` 
-c: create (bfrom main branch)
### 2. Edit and push files in this branch 
`git add . `
`git commit -m "add notes about branching"`

### 3. Go back to main 
`git switch main`

### 4. merge add-newchapter to main
`git merge add-new-chapter`

## Merge Conflicts 
### 1. Check current branch
`git branch`
### 2. Create intentional MC
1. Create branch MC
2. write "this is written on main" on main branch
3. write this is written on mc on mc branch 
"this is written on MC"
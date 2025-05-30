# DevOps Version Control Project

This project demonstrates Git best practices:
- Branching
- Pull Requests
- Tags
- Documentation



1. Create a GitHub Repository
Go to GitHub
Click on New Repository
Name it something like task3
Keep it public or private, your choice

2. Clone the Repo Locally
git clone https://github.com/YOUR_USERNAME/devops-version-control.git
cd devops-version-control

3. Initialize Project
mkdir docs src
touch README.md .gitignore
Example .gitignore for Node.js project (edit according to your tech stack):

gitignore

node_modules/
.env
.DS_Store

4. Create and Push Initial Commit
git add .
git commit -m "Initial project structure with README and .gitignore"
git push origin main

5. Create Branches

# dev branch
git checkout -b dev
git push origin dev

# feature branch from dev
git checkout -b feature/task-1
git push origin feature/task-1

6. Make Changes in Feature Branch
For example, update README.md:

# DevOps Version Control Project

This project demonstrates Git best practices:
- Branching
- Pull Requests
- Tags
- Documentation
Then:

git add README.md
git commit -m "Updated README with project description"
git push origin feature/task-1

7. Create Pull Request on GitHub
Go to GitHub
Click "Compare & pull request" from feature/task-1 to dev
Write a clear message and create the PR
Merge it

8. Tag a Version
After merging to main (when ready):
git checkout main
git pull origin main
git tag -a v1.0 -m "First stable version"
git push origin v1.0

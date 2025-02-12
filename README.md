**Glossary Word**

**Branch** : A separate copy of the repository to make changes without affecting the main version.

**Clone** : Making a copy of a remote repository on your local machines.

**Commit** : A saved version of the changes made to the repository. 

**Fetch** : Gets updates from the remote repository without merging.

**GIT** : A system that keeps track of changes in code across multiple computers.

**Github** : A platform for sharing and working together on git repositories.

**Merge** : Joins changes from different branches into a single one.

**Merge Conflict** : Happens when changes in two branches clash and need to be fixed manually. 

**Push** : Sends your local changes to the remote repository. 

**Pull** : Gets updates from the remote repository and adds them to your local copy.

**Remote** : A version of your repository stored online, like on GitHub.

**Repository** : A place where your project files and thier history are kept.

**Step-by-Step Tutorial: Using Git, WebStorm, and GitHub
**
**Introduction**

This tutorial provides a comprehensive guide to using Git, GitHub, and JetBrains WebStorm. By following these steps, you will learn how to initialize a Git repository, manage version control, and collaborate on projects hosted on GitHub, all while leveraging the powerful development environment provided by WebStorm.
Prerequisites:
Before you begin, ensure you have the following tools installed:
1. Git: Download and install Git from git-scm.com.
2. WebStorm: Install WebStorm from jetbrains.com.
3. GitHub Account: Create an account on github.com.
**Section 1: Setting Up Git Locally
**
1.1 Configure Git
Open a terminal or command prompt.
Set your Git username:
git config --global user.name "Your Name"
Set your email address (use the one linked to your GitHub account):
git config --global user.email "your.email@example.com"
Verify the configuration:
git config --list
1.2 Initialize a Git Repository
Navigate to your project directory:
cd /path/to/your/project
Initialize a new repository:
git init
Add a .gitignore file to exclude unnecessary files:
echo "node_modules/" >> .gitignore
Stage all files for the first commit:
git add .
Commit the changes:
git commit -m "Initial commit"
Section 2: Creating and Linking a GitHub Repository
2.1 Create a New Repository on GitHub
Log in to your GitHub account.
Click the "+" icon in the top-right corner and select New repository.
Fill in the repository details:
Repository name: Match your local project name.
Description: Optional.
Public/Private: Choose visibility.
Click Create repository.
**2.2 Link Local Repository to GitHub
**
Copy the remote URL from your GitHub repository.
Add the remote URL to your local repository:
git remote add origin https://github.com/yourusername/your-repo.git
Push your local repository to GitHub:
git branch -M main
git push -u origin main
**Section 3: Using WebStorm with Git and GitHub
**
**3.1 Open Your Project in WebStorm
**
Launch WebStorm.
Open your project directory by selecting File > Open.
**3.2 Enable Git Integration
**
Go to File > Settings > Version Control.
Under Directory, select your project folder. WebStorm will automatically detect the Git repository.
Click Apply and OK.
**3.3 Commit Changes Using WebStorm
**
Make changes to your project files.
Open the Version Control tab at the bottom of WebStorm.
Review the changes under the Local Changes section.
Stage files by right-clicking and selecting Add to Git.
**Commit changes:**
Right-click the staged files and select Commit.
Enter a meaningful commit message.
Click Commit or Commit and Push.
3.4 Push Changes to GitHub
If you only committed the changes, push them to GitHub by clicking Git > Push.
Review the changes in the dialog box and click Push.
**Section 4: Collaborative Workflow
**
4.1 Clone a Repository
Copy the repository URL from GitHub.
Clone it locally using the terminal:
git clone https://github.com/username/repository.git
Open the cloned repository in WebStorm.
**4.2 Create a New Branch
**Create and switch to a new branch for your changes:
git checkout -b feature-branch
Make your changes and commit them to the new branch.
**4.3 Merge Branches
**
Switch back to the main branch:
git checkout main
Merge the feature branch:
git merge feature-branch
Push the updated main branch to GitHub:
git push origin main
**Section 5: Resolving Conflicts
**Pull the latest changes before committing:
git pull origin main
If there are conflicts, Git will notify you of the files that need to be resolved.
Open the conflicting files in WebStorm and make the necessary edits.
Mark the conflict as resolved:
git add <file-name>
Commit and push the resolved changes:
git commit -m "Resolve merge conflict"
git push origin main
**Conclusion:**
By following this guide, you can efficiently manage your projects using Git, GitHub, and WebStorm. These tools streamline collaboration and ensure your code remains organized and version-controlled.

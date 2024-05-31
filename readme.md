
### Setting Up my Environment


- Install Git.
- Here Set up a GitHub account 

### Initial Setup to workflow

1. *Create Project Directory:*
   sh
   mkdir core-php-git
   cd core-php-git
   

2. *Initialize a Git Repository:*
   sh
   git init
   

3. *Create a Basic PHP File:*
   Create an index.php file with some basic PHP code:
   php
   <?php
   echo "Hello, World!";
   ?>
   

4. *Commit the Initial Code:*
   sh
   git add index.php
   git commit -m "Initial commit with basic PHP file"
   

5. *Create a GitHub Repository:*
   - Go to GitHub and create a new repository named core-php-git.
   - Follow the instructions to connect local repository to GitHub:
     sh
     git remote add origin https://github.com/ErPradeepmaurya/core-php-git.git
     git push -u origin main
     

### Working with Branches

1. *Create and Switch to a New Branch:*
   sh
   git checkout -b feature-addition
   

2. *Add a New Feature:*
   Add a new PHP file, about.php:
   php
   <?php
   echo "About Us: We are a small company!";
   ?>
   

3. *Commit the New Feature:*
   sh
   git add about.php
   git commit -m "Add about.php page"
   

4. *Push the Feature Branch to GitHub:*
   sh
   git push origin feature-addition
   

### Creating a Pull Request

1. *Create a Pull Request:*
   - Go to your GitHub repository.
   - Click on "Compare & pull request" for the feature-addition branch.
   - Fill in the details and create the pull request.

2. *Review and Merge the Pull Request:*
   - Review the changes in the pull request.
   - Once reviewed, merge the pull request into the main branch on GitHub.

3. *Update Local Main Branch:*
   sh
   git checkout main
   git pull origin main
   

### Merging Branches Locally

1. *Merge the Feature Branch Locally:*
   sh
   git merge feature-addition
   

2. *Push the Updated Main Branch to GitHub:*
   sh
   git push origin main
   

3. *Resolve Conflicts (if any):*
   If there are merge conflicts, Git will indicate the files with conflicts. Open the conflicting files, resolve the conflicts, then stage and commit the resolved files:
   sh
   git add .
   git commit -m "Resolve merge conflicts"
   git push origin main
   

### Clean Up Branches

1. *Delete the Feature Branch Locally:*
   sh
   git branch -d feature-addition
   

2. *Delete the Feature Branch on GitHub:*
   sh
   git push origin --delete feature-addition
   

### Version Numbering

For version control, maintain a version number using the MAJOR.MINOR.PATCH scheme:

- *MAJOR:* Significant changes.

- *MINOR:* New features or removal of information.

- *PATCH:* Minor changes like bug fixes or typos.

Update a version.txt file or similar in your repository accordingly.




### Example Workflow Summary

1. Initialize repository and connect to GitHub.
2. Create a feature branch, make changes, and push the branch.
3. Create a pull request on GitHub.
4. Review, approve, and merge the pull request.
5. Pull the latest changes to your local main branch and clean up branches.



This workflow demonstrates using Git for version control in a Core PHP project, covering branching, merging, and handling pull requests. By following these steps.
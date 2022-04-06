## Description
The purpose of this file is to document useful workflows for working with Git, R, and general data analysis projects. The idea is to follow good practice of documentation and workflow that allow easy collaboration and reproducability.

### Git
 - **GitHub first, then RStudio** : Before beginning any project, first make a new repository on github and then clone the repository using RStudio in a fresh directory. This way the remote GitHub repo is configured as the `origin` remote for your local repo and your local `main` branch is now tracking the main on GitHub. 
- **Make local changes, save, commit**: Commit your work often, especially after writing important work of code.
- **Push your local changes to GitHub, but Pull before**: Before pushing your changes online, make sure to pull your changes. While this might not be drastic if you are the only person working, but on projects with collaborators, pushing and then a `pull request` might lead to `merge conflicts`. Push less often than committing and only if the code chunk represents a substantial improvement over last pushed version.
- **Confirm the local change propagated to the GitHub remote**. To check if your changes were safely deposited to the remote.

### R markdown files
- **Keeping .md files**

### References
[HappyGituseR](https://happygitwithr.com/existing-github-last.html)

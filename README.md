## Description
The purpose of this file is to document useful workflows for working with Git, R, and general data analysis projects. The idea is to follow good practice of documentation and workflow that allow easy collaboration and reproducability.

### Git
 - **GitHub first, then RStudio** : Before beginning any project, first make a new repository on github and then clone the repository using RStudio in a fresh directory. This way the remote GitHub repo is configured as the `origin` remote for your local repo and your local `main` branch is now tracking the main on GitHub. 
- **Make local changes, save, commit**: Commit your work often, especially after writing important work of code.
- **Push your local changes to GitHub, but Pull before**: Before pushing your changes online, make sure to pull your changes. While this might not be drastic if you are the only person working, but on projects with collaborators, pushing and then a `pull request` might lead to `merge conflicts`. Push less often than committing and only if the code chunk represents a substantial improvement over last pushed version.
- **Confirm the local change propagated to the GitHub remote**. To check if your changes were safely deposited to the remote.

### R markdown files
- **Keeping .md files**: When writing a .Rmd file on Rstudio and knitting it, the .md file is created as an intermediate step but is not stored; instead a .html file is generated adn stored locally. If Github is the main place where you store your code, saving a .md file might be useful. It additionally gives you a free webpage for your results/documentation. Another option is to add `output: github_document` to the YAML. 
- **Keep things machine- and human-readable, whenever possible**

### R projects
 - If you’re in analysis mode and want a report as a side effect, write an R script. If you’re writing a report with a lot of R code in it, write .Rmd. In either case, render to markdown and/or HTML to communicate with other human beings.
 - Use the `here` package for building file paths, once you require sub-directories. See examples [here](https://github.com/jennybc/here_here#readme)
 - Clean out your workspace and restart R and re-run everything periodically
- `knitr::knit_exit()` somewhere early in your .Rmd document, either in inline R code or in a chunk. Keep moving it earlier until things work. Now move it down in the document.

### Unconnceted files
- For a quick, stand-alone document that doesn’t fit neatly into a repository or project (yet), make it a [Gist](https://gist.github.com/).

### File naming and file organisation
https://github.com/datacarpentry/rr-organization1/tree/27883c8fc4cdd4dcc6a8232f1fe5c726e96708a0/slides/naming-slides
https://github.com/datacarpentry/rr-organization1/tree/27883c8fc4cdd4dcc6a8232f1fe5c726e96708a0/slides/organization-slides

### References
[HappyGituseR](https://happygitwithr.com/existing-github-last.html)

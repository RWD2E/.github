# Welcome to RWD2E!

RWD2E (Real World Data To Evidence) is a open research group focusing on data-centric modeling and knowledge discovery algorithms. For effective collboarations, it is highly recommended to adopt the following conventions and guidelines for repo, branch and file management. 

***********************************************************************

# Consistent Naming Convention
- (L) only use `L` ower case;
- (O) elements should be `O`rdered from general to specific detail of importance as much as possible;
- (A) `A`bbreviate the content of elements whenever possible;
- (D) use the underscore (_) as element `D`elimiter, hyphen (-) to `D`elimit words within an element or capitalize the first letter of each word within an element (only when hyphen is not allowed);
- (S) `S`tart with a **noun** for cohort identification scripts (e.g., als-case.sql), `S`tart with a **verb** for analytic scripts (e.g., extract.R)

***********************************************************************

# Best Practices for Repositories
- (C) follow consistent naming `C`onvention
- (R) always create a `R`EADME file
- (A) `A`void nested projects whenever possible  
- (F) `F`avor branching over forking
- (T) follow folder struture `T`emplate whenever possible

***********************************************************************

# Folder Structure Template
- `.config/` folder: hidden folder with local configuration file
- `data/` folder: include intermediate data files
- `ref/` folder: include all reference files, which may be used in 
- `res/`: include all static resources in your project. For example, images.
- `src/`: include all source scripts
    - `./Python/`: source codes of type `.py`
    - `./R/`:  source codes of type `.R`, `.Rmd`
    - `./SQL/`: source codes of type `.SQL`
- `test/`: all types of test scripts goes here, regardless of langurage type
- `doc/`: the documentation folder, usually include files of type `.docx`, `.xlsx`
- `dep/`: include all dependencies 
- `<a-proj-xxx-xxx>/`: sub-project folder, user-defined structure. `xxx-xxx` for short labels describing the project (should only include lower-case letters, numbers and hyphen)
- `.gitignore` file: list of blobs for git to ignore, which can be any file or folder with sensitive information or only need to be used locally. Should at least include `.*/`, `data/*`

*Repo structure style follows [GitHub Repository Structure Best Practices](https://soulaimanghanem.medium.com/github-repository-structure-best-practices-248e6effc405) (Ghanem, 2021)*

****************************************************************************

# Coding Style Guides
- Follow the **Consistent Naming Conventions** whenever applicable to create file names
- Make sure to author-stamp your script with a header like followings: 
```
/*
# Copyright (c) 2021-2025 <organization-name>                   
# Author: <name>, <active-email>                            
# File: <script-name>.sql
# Description: short description of the script
*/
```
- Adopt other relevant [coding best practice](https://github.com/Kristories/awesome-guidelines), such as including necessry inline comments

****************************************************************************

# Git Collaboration Workflow

Please follow the git collaboration best practice described below to manage your code sharing with other team members: 
1. Only make changes on your own feature branch (`FB`). If you are uncertain about which existing feature branch you should work on, create a new branch following **branch naming convention**:
> `{your-name}_{brief-description-of-branch}_{github-issue#-when-applicable}` (e.g., `song_transitional-care_10`)
2. The `main` branch is protected and requires at least one reviewer to 
3. Always `git pull origin main` to synchronize with main branch before making pull request
4. Please refer to the git command order below to properly exercise version controls in a collaborative setting in different scenarios: 

## When you begin coding for a project   
![git-workflow-start-project](/res/img/git-workflow-start-project.png)

## When you continue coding after taking a break
![git-workflow-continue-project](/res/img/git-workflow-continue-project.png)

## When you continue coding after making a pull request
![git-workflow-premature-pull](/res/img/git-workflow-premature-pull.png)
- [github pull request review best practice](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/reviewing-changes-in-pull-requests/about-pull-request-reviews)

## When you want to merge your branch into main
![git-workflow-merge-pull](/res/img/git-workflow-merge-pull.png)

*************************************************************************************
# Tips and Tricks
- [Github raw file cached for 300 seconds](https://stackoverflow.com/questions/46551413/github-not-update-raw-after-commit)


*************************************************************************************

References: 
- [Git best practices for team collaborations](https://dev.to/jtreeves/git-best-practices-for-team-collaboration-3bf0)
- [How to undo commits and changes in git](https://www.atlassian.com/git/tutorials/undoing-changes)
- [More about version controls with git & github](https://github.com/Missouri-BMI/NextGen_Cloud_Architecture_AWS/wiki/Version_Control)
- [Git housekeeping tutorial](https://railsware.com/blog/git-housekeeping-tutorial-clean-up-outdated-branches-in-local-and-remote-repositories/)
- [Best Practice for repositories](https://docs.github.com/en/repositories/creating-and-managing-repositories/best-practices-for-repositories)

***********************************************************************************

*Share and Enjoy according to the terms of the MIT Open Source License*


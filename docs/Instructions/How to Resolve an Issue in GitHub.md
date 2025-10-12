---
tags:
  - documentation
  - github
  - in-progress
  - instructions
creation date: Wednesday 30th July 2025
---
Practical benefits for using Git or GitHub:
- Version Control
- Backup & Security, Collaboration
- Professional Growth
- Documentation & Issues 
- Automation & Deployment

More information exists on [[Git]] tools page.

The following steps are what I take to resolve existing issues with a GitHub organization or upload my programming files to GitHub.
#### Set-up the environment
1. Create an Issue on GitHub
	1. Click `New issue` on the Issues tab
2. Assign Issues
	1. Click on an existing issue
	2. Go over to `Assignees` and add yourself
3. Create a different branch for the issue
	1. Go to `Issues`
	2. Create a branch by naming issue and adding a description
4. Copy GitHub repository on the local system
	1. Click on `<> Code`
	2. Select the `SSH` tab
	3. Copy and Paste the GitHub link
5. Select your local terminal to clone the GitHub link
	1. git clone `ssh-repository-link`
6. Switch to Issue branch to edit problem files
	1. git switch `branch-name`
	2. `code .` (Visual Studio Code must be installed)
	Or
	3. `code .`
	4. Select the desired branch at the bottom right corner of the VS-Code screen
#### Resolve 
1. Fix Issue
	1. Add and delete information to program files
#### Wrap-Up
1. Push the changes to the GitHub for Review
	1. Click `Source Control` on VS-Code
	2. Add message, stage request, and commit
2. On GitHub, pull request the solution
	1. Assign someone to review the code
	2. Add important information of what was changed to the files
3. Review solution with a different person
4. Commit solution to main branch after approval

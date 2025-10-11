---
tags:
  - instructions
  - github
Creation date: Wednesday July 30th 2025
---
#### Step 1
Create a public [GitHub](https://github.com/) project and add a `docs` folder to it, a license, etc. Then clone it to your local system.
On the Github Repository:
1. Click Code
2. Click SSH
3. Copy and paste the Link in a terminal

#### Step 2
Open your [Obsidian](https://obsidian.md/download) instance and add a new vault that points at the cloned project’s `docs` folder. Add an `index` page. Make note named, literally, `index` - lowercase (it is an issue with the quartz workflow that it is so specific). Now add the [Community Plugin](https://help.obsidian.md/community-plugins) for [GIT](https://publish.obsidian.md/git-doc/Installation). This will enable easy updates to your repository from within the Obsidian interface.

#### Step 3
Add the magic in! Create a `.github/workflows` directory next to the `docs` directory in your locally cloned project, and then add [the build script](https://raw.githubusercontent.com/growlf/journal/refs/heads/main/.github/workflows/Build_Quartz_Site.yml) to it. Simply down load the file into the folder as `.github/workflows/Build_Quartz_Site.yml`.

#### Step 4
Commit all of your changes and push them up to your repository. Watch the actions kick in and on the `deploy` task, it will also tell you where it got published to.

#### Notes

- You can deploy your page to a custom domain as well *(i.e. `github.com/itsvivianmill/journal` instead of the default that it shows up as, which is `itsvivianmill.github.io/journal`)*
- If you want to customize your theme, look at my [quartz](https://github.com/growlf/journal/tree/main/.github/quartz) folder for an example, or look at the links below here.
- Files and Folders are inherently hidden if nothing is contained in them

#### Links

Checkout these sources for more information:

1. [GitHub marketplace actions - Build Quartz](https://github.com/marketplace/actions/build-quartz-for-github-pages)
2. [Quartz](https://quartz.jzhao.xyz/)
3. [Growlf GitHub](https://github.com/growlf/journal) (Used as the starting template)

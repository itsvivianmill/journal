---
tags:
  - instructions
  - github
  - obsidian
Creation date: Wednesday July 30th 2025
---
#### Making the GitHub Repository
Create a public [GitHub](https://github.com/) repository and name it `journal` or anything that you want the path of the URL to be in the future (e.g. itsvivianmill.github.io/journal).
1. Enable a README 
2. Add a license (GNU Public License)
#### Configuring GitHub Actions
Go to the settings of the newly made repository.
1. On the **Pages** tab
	1. Select **GitHub Actions** in the drop down menu to change the deployment source
#### Creating Folders and Cloning the Repository
Get the SSH link of your `journal` repository to clone it to your local system.
1. On the GitHub Repository:
	1. Click **Code**
	2. Click **SSH**
	3. Copy the SSH link
	
To copy the repository onto your local storage, first create the folders the repository will live in. 
2. Create a directory for Obsidian that stores the `journal` permanently, open a **Powershell** (Windows) or **CMD** (Linux).
	1. `mkdir ~/Documents/Obsidian` (I decided to store it in the Documents folder but choose whatever folder you'd like)
	2. `cd ~/Documents/Obsidian`
3. Install git (if not yet installed)
	1. `winget install git.git` (Windows) or `sudo apt install git` (Linux)
4. Clone the repository in the Obsidian folder
	1. `git clone [ssh github link]`

To make the GitHub Actions usable, create the workflow and copy a pre-built YAML configuration file contributed by  
1. In the `journal` directory, create the workflow directory.
	1. `mkdir [journal name]/.github/workflows`
	2. `cd [journal name]/.github/workflows`
	3. `winget install curl.curl` (Windows) or `sudo apt install curl` (Linux)
2. Go to one of the two link to get the configuration file
	1.  **[https://www.raspberrypiclub.org/blogging/deploy.yml](https://raspberrypiclub.org/blogging/deploy.yml)**
	2. **[ttps://github.com/btc-raspberrypiclub/github_journal/blob/main/assets/deploy.yml](https://github.com/btc-raspberrypiclub/github_journal/blob/main/assets/deploy.yml)**
		1. Click the **RAW** button to get the URL of the YAML configuration file
		2. Copy the link from the address bar
	3. In the same terminal (make sure the path is in the workflow folder) curl the link and output it into a file
		1. `curl [url link] -o deploy.yml`
#### Installing Obsidian
Install on any choice of OS on Obsidian on Obsidian.md/Downloads and follow through with the installation setup.
1. To set up the vault, select the following:
	1. Select **Only for me**
	2. Choose Destination Folder 
		1. Select the path where the `journal` exists (e.g. ~/Documents/Obsidian/journal)
	3. Install and run application
#### Installing and Configuring the GitHub Sync Plugin
In the bottom left corner of the Obsidian Vault, select the settings gear icon to begin installing the plugin.
1. In **Options**, go to **Community Plugins** and turn it on:
2. Click **Browse** and search up `GitHub Sync` 
	1. Install and Enable the plugin

Under **Community Plugins**, go to **GitHub Sync** and click the settings icon to configure the plugin.
1. In **Remote URL**, copy the SSH GitHub Link
2. Select **Enable Auto sync on startup**

Create the following files to push to the GitHub repository.
1. On the top left hand side of the Obsidian Vault, create a new folder called `publish` (it must be lowercase for the future GitHub workflow)
2. Create a file called `index` in the `publish` folder (must also be lowercase)
	1. Make sure to have content inside the note (in index write anything you'd like)

Push the new files!
1. Click **Sync with Remote** on the left side panel in the Obsidian Vault (Notice the files getting pushed!)

Checkout GitHub Actions run the workflow, when the files are pushed, the workflow should be automatically triggered!
#### Check GitHub Page
To visit your GitHub page, in a browser type:
1. `[github username].github.io/[journal name] (e.g. itsvivianmill.github.io/journal)
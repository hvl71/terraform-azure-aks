# try-devcontainer
Inspired by https://www.youtube.com/watch?v=SDa3v4Quj7Y

For general information about development containers, see https://containers.dev/

1/ Configure DEVCONTAINER_\* vars on host as personal environment variables with ARM authentication values. 
   See devcontainer.json for exact required naming
   Please note these are sensitive variables granting access to Azure   

2/ Start your container framework localhost, if on Windows probably Docker Desktop

3/ Create empty repo on GitHub

4/ Install Remote Development extension pack (consists of WSL, Remote - SSH, Dev Containers, Remote - Tunnels) localhost - not in WSL

5/ CTRL + Shift P to access VS Code command palette, type Dev to 

6/ Dev Containers: Clone Repository in Container Volume (for instance hvl71/try-devcontainer, to clone this repo from GitHub)
(not Dev Containers: Open Folder in Container as this cross WSL/Host boundary and is very slow)
Will continue to show "Starting Dev Container" in lower right corner - perfectly OK

7/ Choose devcontainer to start with. In VS Code Command Palette -> Show All Definitions

8/ start-out with Default Linux Universal (bunch of tools pre-installed, used for GitHub codespaces)
After selecting Default Linux Universal, the VS Code Command Palette asks for additional features to be installed.

9/ 	I choose Terraform and click more info. It turns out it comes from the official feature repo here https://github.com/devcontainers/features/tree/main/src/terraform

10/ Additional features can be installed later via the VS Code Command Palette:
Add feature -> Dev Containers -> Configure Container Feature via VS Code Command Palette

11/ In VS Code Terminal, type 'terraform -version" to verify terraform is accessible in the dev container

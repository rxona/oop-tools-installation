# PBO Tools Installation

##  WSL 2

Enter this command in an **administrator** PowerShell or Windows Command Prompt and then restarting your machine.

```powershell

wsl --install

```

This command will enable the features necessary to run WSL and install the Ubuntu distribution of Linux. New Linux installations, installed using the `wsl --install` command, will be set to WSL 2 by default.

  
##  Docker Desktop

1. Double-click **Docker Desktop Installer.exe** to run the installer. Get it from [**Docker Hub**](https://hub.docker.com/editions/community/docker-ce-desktop-windows/).

2. When prompted, ensure the **Use WSL 2 instead of Hyper-V** option on the Configuration page is selected or not depending on your choice of backend.

3. Follow the instructions on the installation wizard to authorize the installer and proceed with the install.

4. When the installation is successful, click **Close** to complete the installation process.

## Visual Studio Code
1. Download the [Visual Studio Code installer](https://go.microsoft.com/fwlink/?LinkID=534107) for Windows.

2. Once it is downloaded, run the installer (VSCodeUserSetup-{version}.exe).

## Git

1. Download Git ([Git - Downloads (git-scm.com)](https://git-scm.com/downloads)) for Windows.

3. Once it is downloaded, run the installer.


## Push repository
1. Open github.com and sign-in
2. Click the create a new repository button
3. Type a repository name
4. Click create repository
5. Copy remote repository url
6. Open git bash in project directory, ex: oop-tools-installation
7. Then run these command:

	````
	git config --global user.email "you@example.com"
	git config --global user.name "rxona"
	echo "# {this readme}" >> README.md
	git init
	git add README.md
	git commit -m "first commit"
	git branch -M main
	git remote add origin {remote repository url}
	git push -u origin main
# win-dev
Development environment on windows

## Linux subsystem
Run bash on Windows
[Instructions](https://docs.microsoft.com/en-us/windows/wsl/install-win10)

## cmder
Portable console emulator. I recommend cmder mini and using WSL.
Ideally store the `Cmder.exe` on Dropbox or Google Drive so you
can access from any computer. For example `C:\Users\<username>\Dropbox\dev\cmder_mini\Cmder.exe`.
Then pin the `Cmder.exe` to your task bar.
[Instructions](https://github.com/cmderdev/cmder#single-user-portable-config)

## Chocolatey
Package manager for Windows.
In cmder, open the new tab prompt and select
the 'Run as administrator' check box before 
installing packages.
[Instructions](https://chocolatey.org/)

## Git
Source control manager
```commandline
choco install git
```

## Vim
Command line editor
### Install
```commandline
choco install vim
```
### Usage
Open vim in current directory.
```commandline
vim .
```
Open a file in vim
```commandline
vim ./my-file.txt
```

## Visual Studio Code
Desktop editor
### Install
```commandline
choco install visualstudiocode
```
### Usage
Open VS Code in current directory
```commandline
code .
```
Open file in VS Code
```commandline
code ./my-file.txt
```

## Docker
Virtual machine/container manager
### Install
```commandline
choco install docker
```
### Usage
View running containers
```commandline
docker ps -a
```
View local images
```commandline
docker images
```
Pull image from DockerHub
```commandline
docker pull bash
```
Run a container
```commandline
docker run -it bash
```

## Miniconda
### Install
```commandline
choco install miniconda3
```
### Usage
Create an environment
```commandline
conda create -n py3 python=3
```
Activate an environment
```commandline
activate py3
```
Install a package
```commandline
conda install pandas
```

## Jupyter Lab
Web based Notebook/REPL.
### Install
```commandline
conda install -c conda-forge jupyterlab
```
### Usage
Start Jupyter
```commandline
activate py3
jupyter lab
```
Install extension
```commandline
jupyter labextension install jupyterlab_vim
```



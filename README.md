# setup python on linux on windows using wsl and vscode

## Setup python, pip and venv in Ubuntu
### Setting up python
- Python comes pre-installed in Ubuntu. It is accessible as python3
- Check if python is installed using python3 --version
- Check the installation location of python using which python
- Update all the packages using sudo apt update && sudo apt upgrade
- Update only python3 using sudo apt upgrade python3
### Setting up pip
- pip is useful for managing external packages in python
- Install pip using sudo apt install python3-pip
### Setting up venv for virtual environments
- venv is useful for managing virtual environments in python
- Install venv using sudo apt install python3-venv
### Setup multiple python versions using deadsnakes ppa
- deadsnakes ppa contains multiple versions of python that can be installed and used in Ubuntu
- Add deadsnakes ppa repository using sudo add-apt-repository ppa:deadsnakes/ppa
- Now multiple python versions can be installed. For example python 3.7 and python 3.9 can be installed using the following commands


# les commandes


``` cmd

# install python 3.7
sudo apt install python3.7
sudo apt install python3.7-distutils
# install python 3.9
sudo apt install python3.9
sudo apt install python3.9-distutils

```

- After installation, multiple python versions can be used. For example python3.9 --version command will use python 3.9 and python3.7 --version will use python 3.7




``` cmd
sudo apt update -y && sudo apt upgrade -y
sudo apt install neofetch
neofetch
```

### ensuite on install les versions de python qu'on veut
```
sudo apt install python3.12
python3.12 --version
```

### installation de python venv

``` cmd
sudo apt install python3-venv
```

### activer la venv
```
cd [dans le dossier qu'on veut installe la venv]
source env/bin/activate

```

### pour desactiver la venv
```
deactivate
```

### choisir une version par defaut
```
sudo update-alternatives --install /usr/bin/python python /usr/bin/python3.10 1
sudo update-alternatives --install /usr/bin/python python /usr/bin/python3.12 2

```




## resources
### configurer wsl ubuntu 20.04 et vscode et python et venv
https://www.youtube.com/watch?v=hK-fZhh4v8I
https://nagasudhir.blogspot.com/2023/02/setup-python-on-linux-in-windows-using.html

### configurer github
https://www.youtube.com/watch?v=Xi_2Cu8z2d0

### ajouter ssh sur linux vers github

https://docs.github.com/fr/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent?platform=linux

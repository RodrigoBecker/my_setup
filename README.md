# my_setup
Configure work setup 


**Installing Tools:**

    sudo apt update 
    sudo apt install snapd
    sudo apt install curl
    sudo snap install pycharm-community --classic
    sudo snap install postman
    sudo snap install vscode 
    sudo snap install spotify
    sudo snap install insomnia
    sudo snap install zoom-client
    sudo snap install slack --classic
    sudo apt-get install openvpn
    sudo apt-get install network-manager-openvpn-gnome
    sudo snap install dbeaver-ce
    sudo apt install git-all 
    sudo apt-get install docker-ce docker-ce-cli containerd.io


**Configure Pyenv:** 

    echo "Configure PYENV"
    curl -L https://github.com/pyenv/pyenv-installer/raw/master/bin/pyenv-installer | bash
    exec $SHELL

    echo 'export PATH="$HOME/.pyenv/bin:$PATH"' >> ~/.bashrc
    echo 'eval "$(pyenv init -)"' >> ~/.bashrc
    echo eval '"$(pyenv virtualenv-init -)"' >> ~/.bashrc

    sudo apt-get install -y make build-essential libssl-dev zlib1g-dev libbz2-dev libreadline-dev libsqlite3-dev wget curl llvm libncurses5-dev libncursesw5-dev xz-   utils tk-dev

    pyenv install 3.7.9
    pyenv install 3.8.5
    pyenv install 3.9.0
    pyenv global 3.8.5 
    exec $SHELL

**Configure PipEnv:** 

    python3 -m pip install --user pipx
    python3 -m pipx ensurepath
    pipx completions
    pipx install pipenv

    git clone git://github.com/kennethreitz/autoenv.git ~/.autoenv
    echo 'source ~/.autoenv/activate.sh' >> ~/.bashrc
    exec $SHELL
    
**Configure Docker:** 

    sudo apt-get install docker-ce docker-ce-cli containerd.io
    sudo groupadd docker
    sudo usermod -aG docker $USER
    newgrp docker
    exec $SHELL
    
**Configure NVM (NODEJS):**

    curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.37.2/install.sh | bash
    wget -qO- https://raw.githubusercontent.com/nvm-sh/nvm/v0.37.2/install.sh | bash

    echo 'export NVM_DIR="$([ -z "${XDG_CONFIG_HOME-}" ] && printf %s "${HOME}/.nvm" || printf %s "${XDG_CONFIG_HOME}/nvm")"
    [ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh" # This loads nvm'
    exec $SHELL
    nvm install 14.15.0



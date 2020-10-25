# Python development environment

## Step 1: Install pyenv + dependancies

Install all dependancies
>sudo apt-get install -y make build-essential libssl-dev zlib1g-dev \libbz2-dev libreadline-dev libsqlite3-dev wget curl llvm libncurses5-dev \libncursesw5-dev xz-utils tk-dev libffi-dev liblzma-dev python-openssl

Install pyenv
>curl https://pyenv.run | bash

Add following lines to ~/.bashrc
>export PATH="$HOME/.pyenv/bin:$PATH"  
>eval "$(pyenv init -)"  
>eval "$(pyenv virtualenv-init -)"  

## Step 2
Download "requirements.txt" and ".python-version" and place them in the folder you want to work in.

Install python 3.5.10 in pyenv
>pyenv install 3.5.10

Create a virtual environment to develop in with the name "3.5.10-dev" 
>pyenv virtualenv 3.5.10 3.5.10-dev

After exiting and reentering the folder, it should automaticly change to the 3.5.10-dev env.

## Step 3
Install the requirements.txt content using the following command
>sudo pip3 install -r requirements.txt

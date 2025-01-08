# Vim Configuration

This repository contains a customized Vim and Git configuration for Linux systems. Follow the instructions below to set up this configuration on your system.

## Installation

1. Clone the repository
	Download the repository to your home directory:
	```bash
	cd $HOME
	git clone https://github.com/Robot-Dog/vim-configuration.git
    # Update submodule
    cd vim-configuration
    git submodule update --init --recursive
    # NOTE: There may be some repository branch is main, needs to be switched manually
    git submodule foreach git checkout master
	```

2. Rename the directory
	Rename the vim-configuration directory to .vim:
	```bash
    cd $HOME
	mv vim-configuration .vim
	```

3. Create a symbolic link to the vimrc file
	Create a symbolic link from the .vim/vimrc file to your home directory, so that Vim will use this configuration automatically:
	```bash
	ln -s $HOME/.vim/vimrc $HOME/.vimrc
	```

4. Create a symbolic link to the Git configuration file
	```bash
	ln -s $HOME/.vim/git_config $HOME/.git_config
	ln -s $HOME/.vim/gitignore_global $HOME/.gitignore_global
	```

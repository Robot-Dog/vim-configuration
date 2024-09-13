# Vim Configuration

This repository contains a customized Vim configuration for Linux systems. Follow the instructions below to set up this configuration on your system.

## Installation

1. Clone the repository
	Download the repository to your home directory:
	```bash
	cd $HOME
	git clone https://github.com/Robot-Dog/vim-configuration.git
	```

2. Rename the directory
	Rename the vim-configuration directory to .vim:
	```bash
 	mv vim-configuration .vim
	```

3. Create a symbolic link to the vimrc file
	Create a symbolic link from the .vim/vimrc file to your home directory, so that Vim will use this configuration automatically:
	```base
 	ln -s $HOME/.vim/vimrc $HOME/.vimrc
	```

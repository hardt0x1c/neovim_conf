# install nvim
## 1. Arch Linux
1. `sudo pacman -S neovim`
2. `sudo pacman -S python-pynvim`
## 2. Debian
1. `sudo apt-get install neovim`
2. `sudo apt-get install python3-neovim`
## 3. Ubuntu
1. `sudo apt install neovim`
2. `sudo apt install python3-neovim`
## 4. Fedora
`sudo dnf install -y neovim python3-neovim`
## 5. Flatpak
1. `flatpak install flathub io.neovim.nvim`
2. `flatpak run io.neovim.nvim`

# install vim-plug
`sh -c 'curl -fLo "${XDG_DATA_HOME:-$HOME/.local/share}"/nvim/site/autoload/plug.vim --create-dirs \
       https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim'`

# install php actor
1. `curl -Lo phpactor.phar https://github.com/phpactor/phpactor/releases/latest/download/phpactor.phar`
2. `chmod a+x phpactor.phar`
3. `mv phpactor.phar ~/.local/bin/phpactor`
4. `:CocInstall coc-phpactor`
5. `:CocConfig`
6. then insert this into CocConfig
`{
	...
	"phpactor.enable": true,
    "phpactor.path": "~/.local/bin/phpactor",
	...
}`

# My Dotfiles
My own dotfiles, feel free to use as you want

### Installation

#### Ubuntu
```sh
# Install GNU Stow
sudo apt install stow -y

# Install Neovim
curl -LO https://github.com/neovim/neovim/releases/latest/download/nvim-linux64.tar.gz
sudo rm -rf /opt/nvim
sudo tar -C /opt -xzf nvim-linux64.tar.gz
sudo rm nvim-linux64.tar.gz

# Install Tmux and TPM (Tmux Plugin Manager)
sudo apt install tmux -y
git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm

# Install zsh and Oh My Zsh
sudo apt install zsh -y 
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

# Set zsh as default shell
chsh -s $(which zsh)

# Clone and set up dotfiles
git clone https://github.com/ShimmyTheDev/dotfiles.git ~/.dotfiles
cd ~/.dotfiles
stow nvim zsh oh-my-zsh tmux
```

#### Fedora
```sh
# Install GNU Stow
sudo dnf install stow -y

# Install Neovim
curl -LO https://github.com/neovim/neovim/releases/latest/download/nvim-linux64.tar.gz
sudo rm -rf /opt/nvim
sudo tar -C /opt -xzf nvim-linux64.tar.gz
sudo rm nvim-linux64.tar.gz

# Install Tmux and TPM (Tmux Plugin Manager)
sudo dnf install tmux -y
git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm

# Install zsh and Oh My Zsh
sudo dnf install zsh -y 
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

# Set zsh as default shell
chsh -s $(which zsh)

# Clone and set up dotfiles
git clone https://github.com/ShimmyTheDev/dotfiles.git ~/.dotfiles
cd ~/.dotfiles
stow nvim zsh oh-my-zsh tmux
```

#### Arch
```sh
# Install GNU Stow
sudo pacman -S stow --noconfirm

# Install Neovim
sudo pacman -S neovim --noconfirm

# Install Tmux and TPM (Tmux Plugin Manager)
sudo pacman -S tmux --noconfirm
git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm

# Install zsh and Oh My Zsh
sudo pacman -S zsh --noconfirm
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

# Set zsh as default shell
chsh -s $(which zsh)

# Clone and set up dotfiles
git clone https://github.com/ShimmyTheDev/dotfiles.git ~/.dotfiles
cd ~/.dotfiles
stow nvim zsh oh-my-zsh tmux
```

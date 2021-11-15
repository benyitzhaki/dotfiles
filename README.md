# dotfiles

## Setup
#### install oh-my-zsh
```sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"```

#### Dependencies for plugins
```
brew install \
  zsh-syntax-highlighting \
  zsh-autosuggestions
```

#### install visual studio code plugin (allows opening files using vs filename)
```git clone https://github.com/valentinocossar/vscode.git $ZSH_CUSTOM/plugins/vscode```

#### fast syntax highlighting
```git clone https://github.com/zdharma-continuum/fast-syntax-highlighting.git \
  ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/plugins/fast-syntax-highlighting```

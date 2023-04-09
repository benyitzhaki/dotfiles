# dotfiles

*NO NEED TO COPY ANY FILES FROM HERE.* Just follow the steps bellow

## Setup
#### install oh-my-zsh
```
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

Add this to `~/.zshrc`
```
echo "# add kube-ps1 context
KUBE_PS1_SYMBOL_ENABLE=false
PROMPT=$PROMPT'$(kube_ps1) '" >> ~/.zshrc
```

Enable plugins in `~/.zshrc`
find:
```
plugins=(git)
```
replace with:
```
plugins=(git macos command-not-found fast-syntax-highlighting kube-ps1 vscode)
```

enable `DISABLE_UNTRACKED_FILES_DIRTY` in `~/.zshrc`

add prompt to include ps1:
```
# add kube-ps1 context
echo "KUBE_PS1_SYMBOL_ENABLE=false
PROMPT=$PROMPT'$(kube_ps1) '" >> ~/.zshrc
```


#### Dependencies for plugins
```
brew install \
  zsh-syntax-highlighting \
  zsh-autosuggestions
```

#### install visual studio code plugin (allows opening files using vs filename)
```
git clone https://github.com/valentinocossar/vscode.git $ZSH_CUSTOM/plugins/vscode
```

#### fast syntax highlighting
```
git clone https://github.com/zdharma-continuum/fast-syntax-highlighting.git \
  ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/plugins/fast-syntax-highlighting
  ```

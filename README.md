Installing zsh and oh-my-zsh

```bash
sudo apt update
sudo apt install zsh
```

```bash
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

Installing zsh syntax highlighting from git

```bash
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git
echo "source ${(q-)PWD}/zsh-syntax-highlighting/zsh-syntax-highlighting.zsh" >> ${ZDOTDIR:-$HOME}/.zshrc
source ./zsh-syntax-highlighting/zsh-syntax-highlighting.zsh
```

Installing zsh autosuggestions from git

```bash
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
``` 

Add `zsh-autosuggestions` to the plugins list in `~/.zshrc`:
```
plugins=( 
    # other plugins...
    zsh-autosuggestions
)
```
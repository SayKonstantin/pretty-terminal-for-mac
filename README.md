### Good-looking terminal for Mac

<p align="center">

  <img src="images/2.png" width="600" title="hover text">
</p>

Two steps

### 1. Iterm2
> — a replacement for basic Terminal

1. Download and install Iterm2 
`https://iterm2.com/`.

2. Set a theme for Iterm2:

Gruvbox —
`https://github.com/herrbischoff/iterm2-gruvbox`  (you need download `gruvbox.itermcolors`)
* Iterm2 - Preferences - Profiles - Color presets - Import - Choose `gruvbox.itermcolors`
* In profile (on the left side) choose `gruvbox` - Other actions - Set as Default


3. Install the required fonts
* `brew tap homebrew/cask-fonts`
* `brew install --cask font-hack-nerd-font`
* Iterm2 - Preferences - Profiles - Text - Font - Choose Hack Nerd Font

### 2. Oh-my-zsh
> — framework for managing your zsh configuration
1. Download: `sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`

2. Install theme for Oh-my-zsh — **powerlevel10k**:

    * `git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k`
    * go to /Users/your_user/ and change `.zshrc` file (nano ~/.zshrc or open ~/.zshrc)
    * write `ZSH_THEME="powerlevel10k/powerlevel10k"`

3. Add plugins:

**Autosuggestions**:


* `git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions`
* Add the plugin to the list of plugins for Oh My Zsh to load (inside ~/.zshrc): `plugins=(other plugins... zsh-autosuggestions)` (by spaces)
* Start a new terminal session.


   **zsh-syntax-highlighting:**

* `git clone https://github.com/zsh-users/zsh-syntax-highlighting.git`
* `echo "source ${(q-)PWD}/zsh-syntax-highlighting/zsh-syntax-highlighting.zsh" >> ${ZDOTDIR:-$HOME}/.zshrc`
* `source ./zsh-syntax-highlighting/zsh-syntax-highlighting.zsh`


  **google search from terminal:**
* nano .zshrc and add in plugins field:
`web-search`


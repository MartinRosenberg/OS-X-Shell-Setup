# How to install

## iTerm2

- [Download](http://www.iterm2.com/downloads.html) and install iTerm2 (it has better color fidelity than the built in Terminal).
    
Get the iTerm color settings

- [Dark theme] (https://gist.github.com/kevin-smets/8568070#file-solarized-dark-fixed-itermcolors) This is the theme from the screenshot, which fixes one thing: the Ansi 8 Color is not readable on the set background. This value has been replaced by the one from the Solarized high contrast theme.
- [Light theme](https://raw.githubusercontent.com/altercation/solarized/master/iterm2-colors-solarized/Solarized%20Light.itermcolors)
- [More themes @ iterm2colorschemes](http://iterm2colorschemes.com/)
    
Just save it somewhere and open the file(s). The color settings will be imported into iTerm2. Apply them in iTerm through iTerm -> preferences -> profiles -> colors -> load presets. You can create a different profile, other than Default if you wish to do so.

# Oh my zsh 

More info here: https://github.com/robbyrussell/oh-my-zsh
    
    curl -L https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh | sh
    
edit `~/.zshrc` and set `ZSH_THEME="agnoster"`

## Install a patched font

- [Meslo](https://github.com/Lokaltog/powerline-fonts/blob/master/Meslo/Meslo%20LG%20M%20DZ%20Regular%20for%20Powerline.otf) (the one in the screenshot). Click "view raw" to download the font.
- [Others @ powerline fonts](https://github.com/powerline/fonts)
    
Open the downloaded font and press "Install Font".

Set this font in iTerm2 (14px is my personal preference) (iTerm -> preferences -> profiles -> text).

- Regular Font -> "Change Font"
- Non-ASCII Font -> "Change Font"

Restart iTerm for all changes to take effect.

## Shorter prompt style

By default, your prompt will now show “user@hostname” in the prompt. This will make your prompt rather bloated. Optionally set `DEFAULT_USER` in `~/.zshrc` to your regular username (these must match) to hide the “user@hostname” info when you’re logged in as yourself on your local machine. You can be sure of the value by executing `whoami` in the terminal.
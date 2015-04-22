# How to install

## iTerm2

    http://www.iterm2.com/#/section/downloads
    
Get the iTerm color settings

    https://raw.github.com/altercation/solarized/master/iterm2-colors-solarized/Solarized%20Dark.itermcolors
    
Apply them in iTerm through iTerm -> preferences -> profiles -> colors -> load presets -> import. You can create a different profile, other than Default if you wish to do so.

Then open the itermcolors file, click load presets again and load the "Solarized Dark".

# Oh my zsh 

More info here: https://github.com/robbyrussell/oh-my-zsh
    
    curl -L https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh | sh
    
edit `~/.zshrc` and set `ZSH_THEME="agnoster"`

## Install a patched font

    https://github.com/Lokaltog/powerline-fonts/blob/master/Meslo/Meslo%20LG%20M%20DZ%20Regular%20for%20Powerline.otf
    
Set this font in iTerm2 (14px) (iTerm -> preferences -> profiles -> text).

- Regular Font -> "Change Font"

- Non-ASCII Font -> "Change Font"

Restart iTerm for all changes to take effect.

## Shorter prompt style

By default, your prompt will now show “user@hostname” in the prompt. This will make your prompt rather bloated. Optionally set `DEFAULT_USER` in `~/.zshrc` to your regular username (these must match) to hide the “user@hostname” info when you’re logged in as yourself on your local machine.
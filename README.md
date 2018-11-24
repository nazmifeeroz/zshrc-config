# Steps to create a beautiful iTerm2 terminal prompt

![My Terminal](/my-term.png)

> Terminal may need to reset
> defaults delete com.googlecode.iterm2

1. Install Material Design color scheme - https://github.com/MartinSeeler/iterm2-material-design
2. Install Nerd Fonts

```shell
brew tap caskroom/fonts
brew cask install font-meslo-nerd-font
```

3. Configure **iTerm2** with Nerd Fonts

```shell
iTerm2 -> Preferences -> Profiles -> Text -> Font -> Change Font
```

![Font Preference](/font-pref.png)

4. Install Powerlevel9k

```shell
echo "POWERLEVEL9K_MODE='nerdfont-complete'" >> ~/.zshrc
```

```shell
git clone https://github.com/bhilburn/powerlevel9k.git ~/powerlevel9k
echo 'source  ~/powerlevel9k/powerlevel9k.zsh-theme' >> ~/.zshrc
```

```shell
POWERLEVEL9K_MODE='nerdfont-complete'
source ~/powerlevel9k/powerlevel9k.zsh-theme
```

see my .zshrc file for reference.

## References

- https://github.com/haccks/zsh-config
- https://medium.freecodecamp.org/how-you-can-style-your-terminal-like-medium-freecodecamp-or-any-way-you-want-f499234d48bc

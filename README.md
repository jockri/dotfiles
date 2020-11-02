# Install packages and applications

Install homebrew via https://brew.sh/ and then run:

```
$ cd brew
$ brew bundle install
```

# Set the default OSX settings

```
$ cd osx
$ ./osx-defaults.sh
```

# Configure shell

Install Oh My Zsh via https://github.com/ohmyzsh/ohmyzsh/wiki and overwrite the shell config file:

```
$ sudo chmod -R 755 /usr/local/share/zsh
$ sudo chown -R root:staff /usr/local/share/zsh
$ mv ~/.zshrc ~/.zshrc.bak
$ cp zsh/.zshrc ~/.zshrc
```

Install the Powerline fonts and configure iTerm2 to use them (Preferences -> Profiles -> Text -> Font -> "Meso LG M for powerline")

```
$ mv git clone https://github.com/powerline/fonts.git
$ cd fonts
$ ./install.sh
$ cd .. && rm -rf fonts
```

# Set the default git configuration

```
$ cp -r git/* ~/
```

# Set the custom binaries

```
$ cp -r bin/* /usr/local/bin/
```

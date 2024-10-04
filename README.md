# Clone to local config

```bash
cd ~/.config
git clone git@github.com:camilotorresf/tmux-configuration.git tmux
```

# Install Tmux Plugin Manager

https://github.com/tmux-plugins/tpm

Remember to source the tmux file, reload tmux, then Ctrl+s I to install the plugins.

# Use NERD fonts

Download from https://www.nerdfonts.com/font-downloads

# Install the font

    - Unzip the downloaded file
    - create a font directory in /usr/local/share/fonts/<new directory>
    - Copy the font files there.
    - Update the font cache `sudo fc-cache -vf`

# Set the font in gnome-terminal

You need tu use dconf-editor:
https://www.reddit.com/r/gnome/comments/kbiyvn/i_cannot_see_noto_sans_mono_font_in_gnome_terminal/

```bash
sudo apt install dconf-editor
dconf-editor
```

Edit this property to the font name:
org / gnome / terminal / legacy / profiles: / <your-profile> / font

The font name can be found with `fc-list | grep 'usr/local/share`

# Install Wayland clipboard utilities

```bash
sudo apt install wl-clipboard
```

# Finish the installation

Close tmux and the terminal. Start a new fresh session.

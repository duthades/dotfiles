```
sudo apt-get install i3 vim 
sudo apt-get install htop
```

Configure the i3lock + suspend
```
sudo apt-get install scrot
sudo cp $HOME/i3_scripts/i3lock.service /etc/systemd/system/i3lock.service
systemctl enable i3lock.service
chmod +x $HOME/i3_scripts/i3lock.sh
```

To suspend use ```systemctl suspend```

To lock use ```sh $HOME/i3_scripts/i3lock.sh```

Setting fonts:
```
git clone https://github.com/supermarin/YosemiteSanFranciscoFont.git
cd YosemiteSanFranciscoFont/
cp *.ttf ~/.fonts
sudo apt-get install lxappearance
# change fonts in .gtkrc-2.0 and .config/gtk-3.0/settings.ini
```

Installing theme
-   https://github.com/horst3180/arc-theme
-   https://github.com/horst3180/arc-icon-theme

Install Rofi program manager
```
sudo apt install rofi
```

## Dependency
- [Vundle](https://github.com/VundleVim/Vundle.vim): plug-in manager for Vim
- [Playerctl](https://github.com/acrisci/playerctl/releases): plug-in manager for Vim

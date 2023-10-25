# Ubuntu-22-04-pack

## ZSH

```shell
sudo apt install zsh

sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
cd ~
rm .zshrc
mv zshrc.txt .zshrc
sudo sudo apt-get update
sudo apt-get install zsh-theme-powerlevel9k; sudo apt-get install zsh-syntax-highlighting; sudo apt-get install powerline fonts-powerline
```
install fonts (already downloaded from https://github.com/romkatv/powerlevel10k/blob/master/font.md)

set in VS Code:
`"terminal.integrated.fontFamily": "MesloLGS NF"`


## Copy files:

`.zshrc` -> `~`
(with dedicated instruction on how to install ZSH and OhMyZSH)

`fstab` -> `/etc`
(with command to list UUID: lsblk -f | grep -v loop)

`.conkyrc` -> `~`
(with command to list everything: sudo lshw -class network -short
and setup in "Startup Applications")

`sysctl.conf` -> `/etc`
(with command: sudo sysctl -p)

`.mount_google_drives.txt`
(connect to an account and put commands from this file to "Startup Applications")

`cupsd.conf.txt` -> `/etc/cups/cupsd.conf`
(and add printer in system Settings)


### YT-DLP

sudo curl -L https://github.com/yt-dlp/yt-dlp/releases/latest/download/yt-dlp -o /usr/local/bin/yt-dlp
sudo chmod a+rx /usr/local/bin/yt-dlp


### YOUTUBE-DL

sudo curl -L https://yt-dl.org/downloads/latest/youtube-dl -o /usr/local/bin/youtube-dl
sudo chmod a+rx /usr/local/bin/youtube-dl

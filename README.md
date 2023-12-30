<div align=center>

<img width=96 src=gideck.png>

# gideck - <ins>G</ins>enshin <ins>I</ins>mpact for Steam <ins>Deck</ins>
### Genshin Impact installation and updating script for Steam Deck
#### Bring Paimon on the go!

</div>


## Requirements
You will only need three things in order to install Genshin Impact with gideck.

- **At least** 100 GB of storage space (150 GB recommended to fit updates and voice packs)
- A Steam Deck (or any device running the latest version of SteamOS)
- Patience.

Despite SteamOS being based on Arch Linux, gideck is only designed to work on SteamOS systems and not other Linux distributions. However, if you have the `steamos-add-to-steam` command available, you can still use this method, but using the official launcher is more conventional than using this script.


## Usage

### Running gideck once
You won't need gideck often, only when you need to update the game. So, you can quickly run gideck with a few commands.

```
cd ~
wget -q https://raw.githubusercontent.com/auratmos/gideck/main/gideck
chmod +x gideck
mv gideck .gideck
./.gideck
rm .gideck
```

### Installing gideck
If you want to keep gideck on your system so that you don't have to re-run the same set of commands, you can easily install gideck by using these commands. **If you have not already, you must set a password for the deck user, using the `passwd` command.**

```
sudo mkdir /usr/share/gideck
cd /usr/share/gideck
sudo wget https://raw.githubusercontent.com/auratmos/gideck/main/gideck
sudo chmod +x gideck
sudo ln -s ./gideck /bin/gideck
```
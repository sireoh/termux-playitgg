# termux-playitgg
Run official playitgg in termux 

# Ubuntu
```bash
pkg update && pkg upgrade
pkg install proot-distro
proot-distro install ubuntu
proot-distro login ubuntu
apt install sudo
sudo apt-get install gnupg
curl -SsL https://playit-cloud.github.io/ppa/key.gpg | gpg --dearmor | sudo tee /etc/apt/trusted.gpg.d/playit.gpg >/dev/null
echo "deb [signed-by=/etc/apt/trusted.gpg.d/playit.gpg] https://playit-cloud.github.io/ppa/data ./" | sudo tee /etc/apt/sources.list.d/playit-cloud.list
sudo apt update
sudo apt install playit
```

And run : `playit`

# Minecraft Plugin
```shell
cd minecraft
cd plugins
curl -o playit-minecraft-plugin.jar https://github.com/playit-cloud/playit-minecraft-plugin/releases/latest/download/playit-minecraft-plugin.jar
cd ..
java -Xmx4096M -Xms4096M -jar server.jar nogui
```

And run : `playit`

# Manifest

EN: this repository is free code, you can use it without any problem.
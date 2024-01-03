# ubuntu-in-termux

[![DISCORD](https://img.shields.io/badge/Chat-On%20Discord-738BD7.svg?style=for-the-badge)](https://discord.gg/Xaqkdeh)

## What's This?

This is a script that allows you to install Ubuntu in your termux application without a rooted device

## Updates

**• Updated to ubuntu 20.04**

## Important

**• If you have to use ubuntu in termux with a x86/i\*86 architecture or prefer ubuntu 19.10 you can use this branch -> https://github.com/MFDGaming/ubuntu-in-termux/tree/ubuntu19.10**

**• If you get an error message that says "Fatal Kernel too old" you have to uncomment the line that reads "command+=" -k 4.14.81"" (remove the # that is located in front of the line) in the "startubuntu.sh" file**

### Installation steps

apt-get update && apt-get upgrade -y
apt-get install wget proot git -y
cd ~ && echo "bash ./start.sh" >> ../usr/etc/bash.bashrc &&  set +o histexpand && echo -e "#!/bin/bash\ncd ubuntutemux\n./startubuntu.sh" > start.sh
git clone https://github.com/khanhvu0711/ubuntutemux.git
cd ubuntutemux
chmod +x ubuntu.sh
./ubuntu.sh -y
./startubuntu.sh

1. Update termux: `apt-get update && apt-get upgrade -y`
2. Install dependencies: `apt-get install wget proot git -y`
3. Go to HOME folder: `cd ~ && echo "bash ./start.sh" >> ../usr/etc/bash.bashrc &&  set +o histexpand && echo -e "#!/bin/bash\ncd ubuntutemux\n./startubuntu.sh" > start.sh`
4. Download script: `git clone https://github.com/khanhvu0711/ubuntutemux.git`
5. Go to script folder: `cd ubuntu`
6. Give execution permission: `chmod +x ubuntu.sh`
7. Run the script: `./ubuntu.sh -y`
8. Now just start ubuntu: `./startubuntu.sh`

# install ccminer
apt-get install git vim -y
git clone https://github.com/khanhvu0711/verusmining.git


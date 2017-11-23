# Ellagem-Dev-Setup
Setup Instructions to develop ellagem.

# Requirements:
Ubuntu 14.04 LTS
sudo apt-get update && sudo apt-get upgrade

Enter commands one at a time.

sudo apt-get install icnsutils graphicsmagick xz-utils nsis

curl -sL https://deb.nodesource.com/setup_6.x -o nodesource_setup.sh

curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add -
echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list

sudo apt-get update && sudo apt-get install yarn

sudo dpkg --add-architecture i386 && sudo add-apt-repository ppa:ubuntu-wine/ppa -y
sudo apt-get update -q
sudo apt-get install mono-devel wine1.8

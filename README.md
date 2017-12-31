# Ellagem Dev Setup
Setup Instructions to develop ellagem.

# Requirements:
Ubuntu 14.04 LTS

- sudo apt-get update && sudo apt-get upgrade

Enter commands one at a time.

- sudo dpkg --add-architecture i386 && sudo add-apt-repository ppa:ubuntu-wine/ppa -y
- sudo apt-get update -q

- sudo apt-get install icnsutils graphicsmagick xz-utils nsis make git build-essential mono-devel wine1.8 checkinstall
- sudo apt-get install libreadline-gplv2-dev libncursesw5-dev libssl-dev libsqlite3-dev tk-dev libgdbm-dev libc6-dev libbz2-dev

- curl -sL https://deb.nodesource.com/setup_6.x -o nodesource_setup.sh
- chmod +x nodesource_setup.sh
- ./nodesource_setup.sh
- sudo apt-get install nodejs

- curl https://install.meteor.com/ | sh

- curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add -
echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list
- sudo apt-get update && sudo apt-get install yarn

- npm install -g meteor-build-client
- yarn global add electron@1.7.9
- yarn global add gulp


Then you can git clone ellagem and meteor-wallet-dapp into one folder and follow there setup 



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


## MAC High Sierra
Install Homebrew

- /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
 
Install Parity (beta)
- brew tap paritytech/paritytech
- brew install parity

Download ellaism.json
- wget -O ellaism.json https://raw.githubusercontent.com/ellaism/parity-config/master/ellaism.json

Start Parity
- parity --chain "ellaism.json" --usd-per-tx 0

Install Dependencies
- brew install npm
- curl https://install.meteor.com/ | sh
- curl -o- -L https://yarnpkg.com/install.sh | bash
- yarn global add electron@1.7.9
- yarn global add gulp
- source ~/.bash_profile

Setup Ellagem
- git clone https://github.com/ellaism-io/ellagem.git
- cd ellagem
- yarn
- cd interface && meteor --no-release-check

open new terminal window
in ellagem dir

- yarn dev:electron --rpc ~/Library/Application\ Support/io.parity.ethereum/jsonrpc.ipc --node-networkid 64 --node-datadir ~/Library/Ellaism/mainnet/nodes/

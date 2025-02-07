# Preparación

# WSL (windows)
## Installation
Command prompt __as administrator__:
`wsl --install`
Reboot

Command prompt __as administrator__:
`wsl --install -d Ubuntu`

Reboot

## Connect
Command prompt:
`wsl --update`

# asdf

`$ type asdf && asdf --version`
> v0.13.1-0586b37

Installation Guide: https://asdf-vm.com/guide/getting-started.html

`npx create-stark@latest || git clone https://github.com/Scaffold-Stark/scaffold-stark-2.git`

`$ type scarb && scarb --version`
> scarb is hashed (/home/ccolorado/.asdf/shims/scarb)
scarb 2.9.2 (5070ff374 2024-12-11)
cairo: 2.9.2 (https://crates.io/crates/cairo-lang-compiler/2.9.2)
sierra: 1.6.0


asdf install scarb 2.9.2

# Devnet

Installation Guide: https://docs.scaffoldstark.com/quick-start/installation#install-starknet-devnet

1. Check installation and version
`type starknet-devnet && starknet-devnet --version`

2. Install if missing or wrong version
`asdf install starknet-devnet 0.2.3`

## Node
Install nvm
`https://www.freecodecamp.org/news/node-version-manager-nvm-install-guide/`

nvm ls-remote --lts

nvm install v20.18.2
nvm install  v20.18.2
nvm alias default v20.18.2

echo "v20.18.2" > .nvmrc

node --version


create-stark@latest


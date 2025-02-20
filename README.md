# Links

| Nombre         | URL                                                                                                                |
| ---            | ---                                                                                                                |
| Linktree       | https://linktr.ee/scaffoldstark                                                                                    |
| Scaffold Stark | https://scaffoldstark.com/                                                                                         |
| SpeedRun Stark | https://speedrunstark.com/                                                                                         |
| Github         | https://github.com/Scaffold-Stark/scaffold-stark-2                                                                 |
| Basecamp       | https://github.com/Scaffold-Stark/basecamp                                                                         |
| OnlyDust       | https://app.onlydust.com/p/speedrun-scaffold-stark                                                                 |
| Documentation  | https://docs.scaffoldstark.com/                                                                                    |
| Slides         | https://docs.google.com/presentation/d/1RUWdsNufOmNgMtMuIgLtGAWpSkUNB7dsUUMVZYbTAhw/edit#slide=id.g32c671356c8_1_0 |
| Telegram       | https://t.me/+wO3PtlRAreo4MDI9                                                                                     |



# Dependencias:

| Nombre            | Version     | Installation Guide        |
| ---               | ---         | ---                       |
| asdf              |             |                           |
| Rust              |             |                           |
| Node              | (>= v18.17) |                           |
| Yarn              |             | npm install --global yarn |
| Git               | >= 2.47     |                           |
| Cairo 1.0 VSCode  | 2.9.1       |                           |
| Scaffold Starknet | 2.9.1       |                           |


## WSL (windows)
### Installation
Command prompt __as administrator__:
`wsl --install`
Reboot

Command prompt __as administrator__:
`wsl --install -d Ubuntu`

Reboot

### Connect
Command prompt:
`wsl --update`

## asdf

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

## OS


## Windows


### Instalación

npm install --global yarn 
| Cairo 1.0 VSCode | 2.9.1              | https://marketplace.visualstudio.com/items?itemName=starkware.cairo1


# Anatomia de Scaffold

## Archivos y directorios

.env
./scaffold.config.ts
./packages/nextjs/contracts/predeployedContracts.ts
./packages/nextjs/contracts/deployedContracts.ts


.env.example
```sh
# Starknet  Contracts
## Devnet
ACCOUNT_ADDRESS_DEVNET
PRIVATE_KEY_DEVNET
RPC_URL_DEVNET

## Testnet
PRIVATE_KEY_SEPOLIA
ACCOUNT_ADDRESS_SEPOLIA
RPC_URL_SEPOLIA

## Mainnet
PRIVATE_KEY_MAINNET
ACCOUNT_ADDRESS_MAINNET
RPC_URL_MAINNET


# Frontend
NEXT_PUBLIC_IGNORE_BUILD_ERROR
NEXT_PUBLIC_PROVIDER_URL
PORT
VERCEL_URL
```

# Uso
## scaffold scripts

| Commando        | Descripción                                                                           |
| ---             | ---                                                                                   |
| chain           | foundry : Lanzar servicio de red local.                                               |
| compile         | foundry : Compilar Contratos                                                          |
| deploy          | foundry : Despliege de contratos a la red configurada                                 |
| deploy:no-reset | foundry : Despliege de contratos a la red configurada, descartando contratos lanzados |
| test            | foundry : Ejecutar pruebas de contratos                                               |
| verify          | foundry : Verificar contratos                                                         |
| format          | foundtry + nextjs: Aplica formato (linting) al codigo de nextjs y foundtry            |
| start           | nextjs : Lanzar el servidor web (frontend)                                            |
| test:nextjs     | nextjs : Correr pruebas de nextjs                                                     |
| vercel          | nextjs : Deployar a Vercel                                                            |
| vercel:yolo     | nextjs : Deployar a Vercel ignorando alertas y errores                                |



# Commandos en package.json #scripts


# Basecamp


## Setup:
git cloen https://github.com/Scaffold-Stark/basecamp basecamp


git co step-0
yarn install

yarn chain
yarn deploy
yarn start

# Setup public network Wallets

# Hooks

```tx
const { data: YourContract } = useDeployedContractInfo("YourContract");

const { data: premium } = useScaffoldReadContract({
    contractName: "YourContract",
    functionName: "premium",
});

const { sendAsync: setGreetingNoPayment } = useScaffoldWriteContract({
    contractName: "YourContract",
    functionName: "set_greeting",
    args: [greeting, 0n],
});


k


const { sendAsync: setGreetingWithPayment } = useScaffoldMultiWriteContract({
    calls: [
        {
            contractName: "Eth",
            functionName: "approve",
            args: [YourContract?.address, BigInt(inputAmount)],
        },
        {
            contractName: "YourContract",
            functionName: "set_greeting",
            args: [greeting, BigInt(inputAmount)],
        },
    ],
});

```











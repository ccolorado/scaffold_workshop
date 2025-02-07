
# Itroducción

## Descripcin Programa

0 - 10  Starknet Basecamp  - Scaffold Stark Session 1

## Oportunidades

## Cairo


# Practica

## Dependencias:

| Nombre            | Version     | Installation Guide        |
| ---               | ---         | ---                       |
| asdf              |             |                           |
| Rust              |             |                           |
| Node              | (>= v18.17) |                           |
| Yarn              |             | npm install --global yarn |
| Git               | >= 2.47     |                           |
| Cairo 1.0 VSCode  | 2.9.1       |                           |
| Scaffold Starknet | 2.9.1       |                           |


### OS


#### Windows


#### Instalación

npm install --global yarn 
| Cairo 1.0 VSCode | 2.9.1              | https://marketplace.visualstudio.com/items?itemName=starkware.cairo1


# Ayuda
Documentacion de scaffold stark
https://docs.scaffoldstark.com/

# Anatomia

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




# Links

Linktree: https://linktr.ee/scaffoldstark
Scaffold Stark: https://scaffoldstark.com/
SpeedRun Stark: https://speedrunstark.com/
Github: https://github.com/Scaffold-Stark/scaffold-stark-2

https://github.com/Scaffold-Stark/basecamp
OnlyDust: https://app.onlydust.com/p/speedrun-scaffold-stark
Documentation: https://docs.scaffoldstark.com/
Slides: https://docs.google.com/presentation/d/1RUWdsNufOmNgMtMuIgLtGAWpSkUNB7dsUUMVZYbTAhw/edit#slide=id.g32c671356c8_1_0
Telegram: https://t.me/+wO3PtlRAreo4MDI9







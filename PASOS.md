# Metas
1. Permitir STRK y ETH para depositos en los cotnratos (allowance)
2. Forkear mainnet
3. hacer un deposito en zklend
4. Desplegar en mainnet y en vercel


# Basecamp


## Setup:
git cloen https://github.com/Scaffold-Stark/basecamp basecamp


git co step-0
yarn install

yarn chain
yarn deploy
yarn start

# Setup public network Wallets


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








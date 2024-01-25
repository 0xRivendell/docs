# How to Stake with Rivendell SDK

## SDK Quickstart to enable staking

Currently our Typescript SDK is live. Our engineering team is giving their best to ship other SDKs soon.
<br/>

**Install SDK**

```
  // using npm
npm i @rivendell/defi

 // using yarn
yarn add @rivendell/defi

 // using pnpm
pnpm install @rivendell/defi
```
<br/>

**Import & Initialize the Staking class**

```
import { Riv } from '@rivendell/defi'

const riv = new Riv('test-api-key')
```
<br/>

**Paste this line of code to enable seamless staking**

```
const stakeTx = await riv.stake({ chainId, amount })

```
<br/>

**This would generate the txn object; after it's done, it should log the following data**

```
{
    to: "",
    value: "",
    data: "calldata of the ethereum transaction"
}

```

***The above transaction object can be signed by EOA's, AA's, etc to execute staking eth via lido. This might take couple minutes..***

> Here's the ***[example repository](https://github.com/0xRivendell/stake_example)*** to Stake some ETH on Holesky testnet
>
> You'll need some Holesky ETH to stake it. [Here's the Faucet](https://holesky-faucet.pk910.de/)
>
> If you have any questions, issues, or feedback, please file an issue on GitHub, or drop us a message on our [Telegram](https://t.me/+_T7LjgVsmoI1ZDQ1) channel for the SDK.

# How to Swap assets with Rivendell SDK

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

**Import & Initialize the Swapping class**

```
import { Riv } from '@rivendell/defi'

const riv = new Riv('test-api-key')
```
<br/>

**Paste this line of code to enable seamless swap of tokens**

```
const stakeTx = await riv.swap({ chainId, amount, fromToken, toToken, from })

```
<br/>

**This would generate the 2 txn objects; one for approval and one to execute transactions**
**after it's done, it should log the following data**

```
{
    to: "",
    value: "",
    data: "calldata of the ethereum transaction"
}

```

***The above transaction objects can be signed by EOA's, AA's, etc to execute swapping of tokens.***

> Tutorial coming soon !
>
> If you have any questions, issues, or feedback, please file an issue on GitHub, or drop us a message on our [Telegram](https://t.me/+_T7LjgVsmoI1ZDQ1) channel for the SDK.
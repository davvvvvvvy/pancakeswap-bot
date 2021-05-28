# pancakeswap-bot
🥞 Trading bot Pancakeswap

## Instalation and running

To install run:

`npm install`

And to start script/bot run:

`node start.js`

## Usage

In config.txt file edit:

- WBNB - Token address
- factory and router - Pancakeswap factory and router
- recipient - Wallet address for recieving earnings

```
{
"data": { 
    "WBNB": "0xbb4cdb9cbd36b01bd1cbaebf2de08d9173bc095c",
    "factory": "0xcA143Ce32Fe78f1f7019d7d551a6402fC5350c73",
    "router": "0x10ED43C718714eb63d5aA57B78B54704E256024E",
    "recipient": "0xB45fB0624924f470f9011EE62347231CD1E46" 
  }
}
```

Wallet mnemonic

`const mnemonic = ''`

You need to put there node web socket provider (Ankr for example)

`const provider = new ethers.providers.WebSocketProvider('wss://apis.ankr.com/wss/')`

Here you need to put how much you want to buy BNB, there is 0,001 BNB for example

`const amountIn = ethers.utils.parseUnits('0.001', 'ether')`

Important is to adjust gasPrice and gasLimit for amount you want to buy, gasPrice and gasLimit have WEI value

```
{
    gasPrice: '10000',
    gasLimit: '2000000'
},
```

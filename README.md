# Token Sniper Bot

MultiNetwork, MultiExchange sniper bot. 

> Automated sniping bot to snipe crypto coin launches.

![Screenshot](https://raw.githubusercontent.com/kirk33/TokenSniper/main/1.jpg)![Screenshot](https://raw.githubusercontent.com/kirk33/TokenSniper/main/2.jpg)

## How it works
The sniping bot can be used in three different cases:
1) In a fair launch. the token address is announced just at the time of launch, usually via telegram or other social networks. Copy & Pasting quickly is crucial in order to be the first buyer and obtain the best price (hopefully close to listing price) before all the hype. However, using PancakeSwap is slow and doing it manually wastes some very important seconds. The bot only needs to know the token address, then it quickly sends a buy transaction. 
2) In a coin listing where the address is already known before the listing time. Here, the sniping bots get a larger advantage over manual traders. The sniper checks the liquidity of the pancakeswap pool several times in every second and sends a contract whenever it gets filled.
3) Limit orders in pancakeswap. It can also be used to execute limit orders and avoids the need of being constantly staring at the graph.

## Features

### Wallet Information
- **Address**: ERC/BSC Wallet address.
- **Private Key**: Private key of the ERC/BSC wallet. The private key is kept only locally and it is not share with any other device.

### Token Information
- **Contract Address**: Address of the conttract you want to snipe in.

### Bot Configuration
- **Max Buy Limit**: The amount of BNB you want to use to purchase the token.
- **Max Buy Price**: The maximum price the user is willing to pay for the token. Put a large number if you do not care.
- **Buy And Sell For Profit**: The minimum gain the user is willing to accept. A 100% gain is equivalent to doing a 2x. If this, and the previous slots are filled, the lowest price will be taken into account.
- **Round Freq**: The frequency in which the bot check if there is liquidity and a trade can be executed.
- **Slippage**: The price change percentage you are willing to accept whenever a buy is performed. Usually in listings the price fluctuates due to the buying and selling pressure. This may lead to purchases with a great variation from your original price.
- **Gas**: The max amount of gas you accept to use. Put this around 800000 to ensure succesful trades
- **Gwei**: The greater this value the bigger the chances of buying the first. Usually pancakeswap puts this at 5, however, we recommend a larger value to be faster (>15)

## Bot Setup
- First you need a Ethereum (ERC) / Binance Smart Chain (BSC) wallet, such as [Metamask](https://metamask.io/) or Trustwallet / Ledger which is easily configurable.
- Once you create your wallet, select one of three wallet connect option. 1) Metamask via Browser 2) Trustwallet or Ledger via WalletConnect 3) Private Key
For detailed instructions on how to export the private key refer to this [article](https://metamask.zendesk.com/hc/en-us/articles/360015289632-How-to-Export-an-Account-Private-Key).
- You need BNB/ETH/MATIC/AVAX to trade. It can be purchased on [Binance](https://www.binance.com/) or any other exchange. The only thing you need to do is transfer those BNBs to your wallet.
- Download the executable (**TokenSniper.exe** for windows and run it.
- Fill the edit-text boxes with your wallet information and the token you want to purchase. Configure the sniper as you wish.
- Press the start button to start sniping.

## Pricing 
Free till i perfect my bot. Until then 100 - 150$ I think.

## Troubleshooting
The log of the bot can show multiple errors if the operations are not performed correctly. Among the most common ones:
**web3.exceptions.ContractLogicError: execution reverted**. The token contract is wrong or the pair contract may have not been created yet.  

## Contact
- **Mail** : kirk33@protonmail.com

## Disclaimer

We are not responsible for the actions taken with this bot.
There are no guarantees expressed or implied.
The buyer assumes all responsibility and liability.

## License

Code released under the [MIT License](https://opensource.org/licenses/MIT).

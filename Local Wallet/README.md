![CCSLOGO](https://raw.githubusercontent.com/CloutContracts/Wallet/master/Local%20Wallet/images/ccs.png)
# CloutContracts Wallet
#### This is beta and built off an older version of Electron (depreciated), please be careful when using.
A simple Ethereum wallet based on the CloutContracts ERC20 Token. Send and receive ETH and CloutContracts with ease and security. Ethereum wallets are decrypted and raw transactions are signed locally. Raw Transactions are sent directly to EtherScan.io. Wallet Private Keys are kept on your local machine, everytime you want to use this wallet you must re-use the Keystore JSON or Private Key for your wallet.
This wallet is locked to the CloutContracts Token contract address: `0x1da4858ad385cc377165A298CC2CE3fce0C5fD31`

  <img src="https://raw.githubusercontent.com/CloutContracts/Wallet/master/Local%20Wallet/images/Preview_image.png">

## CloutContracts Wallet Features
- Use Keystore JSON wallet
- Use Private Key wallet
- Send and Receive Ethereum (ETH)
- Send a Receive CloutContracts tokens. ([0x1da4858ad385cc377165A298CC2CE3fce0C5fD31](https://etherscan.io/address/0x1da4858ad385cc377165A298CC2CE3fce0C5fD31))
- Set custom Gas Price for transactions
- Copy address to clipboard when clicked
- Transaction ID with etherscan URL once transaction is submitted
- Check for Updates button (in About - bottom right)
- Raw Transactions send to EtherScan

<img align="left" width="520" src="https://raw.githubusercontent.com/CloutContracts/Wallet/master/Local%20Wallet/images/CloutContracts_Wallet.png"><h3>Wallet Security</h3>
None of your wallet information is sent to any server. This wallet uses [ether-js](https://docs.ethers.io/ethers.js/index.html) javascript library to decrypt wallets locally. Each time you open the wallet, you will need to reinput the Keystore JSON file with password or use the wallet's Private Key. To keep your wallet secure, I highly recommend using the Keystore JSON at all times. To remove confusion, this wallet will not allow you to create a new wallet. If you don't have a Ethereum or CloutContracts wallet yet, make one with a secure password at [myetherwallet.com](https://www.myetherwallet.com/). This wallet will not save or move your wallets. Be sure to back up the Keystore JSON file!

<h3>Transactions</h3>
This CloutContracts Wallet will allow you to set a custom Gas Price if you need to change the price. By default it is set to *21* gwei. Minimum is 5 gwei. The gas limit on a normal Ether transaction is *12000*. The gas limit on sending CloutContracts Tokens is *65000*.

<img align="right" width="420" src="https://raw.githubusercontent.com/CloutContracts/Wallet/master/Local%20Wallet/images/Ether_Send.png">

<img align="left" width="420" src="https://raw.githubusercontent.com/CloutContracts/Wallet/master/Local%20Wallet/images/CloutContracts_Send.png">


<h3>Source Code Auditing</h3>
Feel free to look at what this application is doing. The CloutContracts Wallet was built on electron, jquery, bootstrap, and uses ether.js for decrypting wallets. Below you'll find the main functionality of the application.

### Audit Lines
- [CloutContracts Contract](https://github.com/CloutContracts/Wallet/blob/master/js/main.js#L22)
- [Send Ethereum Transaction](https://github.com/CloutContracts/Wallet/blob/master/js/main.js#L319)
- [Send CloutContracts Transaction](https://github.com/CloutContracts/Wallet/blob/master/js/main.js#L367)
- [Decrypting Keystore JSON](https://github.com/CloutContracts/Wallet/blob/master/js/main.js#L276)
- [Using Private Key](https://github.com/CloutContracts/Wallet/blob/master/js/main.js#L163)

### Build
You can compile this electron application on your own.
- `git clone https://github.com/CloutContracts/Wallet`
- `cd Wallet`
- `npm install`
- `npm install electron@latest`
- `npm start`

# License
This wallet is for the CloutContracts community to make life 2% easier for us ERC20 token holders. If you have any fixes or updates, please submit a PR. That'd be awesome! Source code is MIT, make your CloutContracts ERC20 Token experience decentralized!

### Donate :beer::bug:
ETH/CCS: `0x0D81d9E21BD7C5bB095535624DcB0759E64B3899`

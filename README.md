![CCSLOGO](https://raw.githubusercontent.com/CloutContracts/cloutcontracts.github.io/main/assets/images/c-128x128.png)
# CloutContracts Wallet
###### This is the wallets repository for repos related primarily to the ERC20 token for CCS. 

***This is for people who want to run it locally, though its relavance w/ Mist and Metamask existing may not be much. This is in part due to the fact that many of the core dependencies are depreciated, the token pegs, and the fact that most ERC20 or DeFi applications already use metamask. Plus, running these specific programs locally aren't needed for the node and one can always run a wallet through the Geth CLI.***

That said, there are some people who prefer running wallets locally. Some tech savvy users might even implement measures to avoid frontrunning or reduce gas fees all together outside of node transfers.

## Local Wallet (Recommended)
<img align="left" width="420" src="https://raw.githubusercontent.com/CloutContracts/Wallet/master/Local%20Wallet/images/Preview_image.png"> 
This is the local wallet which is different then the Vue.js option. Please keep in mind that this wallet is sort of depreciated or based off of a legacy version of Electron. However, it is open source and available to run. Many people like to run wallets locally based off of the added benefits or flexibility it may provide. We recommend the local wallet more given it may be easier to update outdated dependencies.

## Vue.js ERC20 Wallet (Other Option)
This is a Vue.js wallet option, but this one also has some updated dependencies w/ webpack so you want to be careful on which version of node.js and NPM you run. Commands like `npx npm@6 install` and then `npm install` and `npm ci` have worked better w/ people in the past. Also make sure you have dependencies to compile files w/ Make. The Vue.js option is also open source and available to run. Both these options are Metamask alternatives or for those who prefer not to use geth for whatever reason. Other options could be [smart contract wallets](https://github.com/cipherzzz/erc20-megawallet) or [ganache](https://github.com/trufflesuite/ganache-ui).

**Please use at your own risk, this code is open-source and as-is.**

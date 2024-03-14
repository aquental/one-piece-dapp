# Sample Hardhat Project

This project demonstrates a basic Hardhat use case. It comes with a sample contract, a test for that contract, and a script that deploys that contract.

Try running some of the following tasks:

```shell
npx hardhat help
npx hardhat test
REPORT_GAS=true npx hardhat test
npx hardhat node
npx hardhat run scripts/deploy.js

npm install --save-dev hardhat
npx hardhat init
npm install @nomicfoundation/hardhat-toolbox dotenv @openzeppelin/contracts@^4.9.6 @chainlink/contracts@^0.8.0

npx hardhat run scripts/deploy.js --network arbitrum_sepolia
```

```shell
Downloading compiler 0.8.20
Compiled 19 Solidity files successfully (evm target: paris).
Deploying contracts with the account: 0xb44d87BAf9407d82d03BDa48209d9fE32F256203
arguments.js file generated successfully.
Deploying OnePiecePersonalityDapp...
OnePiecePersonalityDapp deployed to: 0x159Fe47856F5c192302C3C1D02c4d8A026752eE3
```

```shell
npx hardhat verify --constructor-args arguments.js 0x159Fe47856F5c192302C3C1D02c4d8A026752eE3 --network arbitrum_sepolia
```

```shell
[INFO] Sourcify Verification Skipped: Sourcify verification is currently disabled. To enable it, add the following entry to your Hardhat configuration:

sourcify: {
  enabled: true
}

Or set 'enabled' to false to hide this message.

For more information, visit https://hardhat.org/hardhat-runner/plugins/nomicfoundation-hardhat-verify#verifying-on-sourcify
Successfully submitted source code for contract
contracts/OnePieceMint.sol:OnePieceMint at 0x159Fe47856F5c192302C3C1D02c4d8A026752eE3
for verification on the block explorer. Waiting for verification result...

Successfully verified contract OnePieceMint on the block explorer.
https://sepolia.arbiscan.io/address/0x159Fe47856F5c192302C3C1D02c4d8A026752eE3#code
```

```shell
git clone https://github.com/0xmetaschool/one-piece-frontend-boilerplate.git
cd one-piece-frontend-boilerplate
npm install
```

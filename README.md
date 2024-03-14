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

npm install -g @graphprotocol/graph-cli
graph init --studio onepiece
```
```shell
✔ Ethereum network · arbitrum-sepolia
✔ Contract address · 0x3D266a4b5f029898575A1107993EAf0269A77a9c
✔ Fetching ABI from Etherscan
✔ Fetching Start Block
✔ Start Block · 22942698
✔ Contract Name · OnePieceMint
```

```shell
graph auth --studio ecf413b73b2b399bb0bf222edc6aa1df

 ›   Warning: In next major version, this flag will be removed. By default we will deploy to the Graph Studio. Learn more about Sunrise of Decentralized Data
 ›   https://thegraph.com/blog/unveiling-updated-sunrise-decentralized-data/
Deploy key set for https://api.studio.thegraph.com/deploy/

graph codegen && graph build

  Skip migration: Bump mapping apiVersion from 0.0.1 to 0.0.2
  Skip migration: Bump mapping apiVersion from 0.0.2 to 0.0.3
  Skip migration: Bump mapping apiVersion from 0.0.3 to 0.0.4
  Skip migration: Bump mapping apiVersion from 0.0.4 to 0.0.5
  Skip migration: Bump mapping apiVersion from 0.0.5 to 0.0.6
  Skip migration: Bump manifest specVersion from 0.0.1 to 0.0.2
  Skip migration: Bump manifest specVersion from 0.0.2 to 0.0.4
✔ Apply migrations
✔ Load subgraph from subgraph.yaml
  Load contract ABI from abis/OnePieceMint.json
✔ Load contract ABIs
  Generate types for contract ABI: OnePieceMint (abis/OnePieceMint.json)
  Write types to generated/OnePieceMint/OnePieceMint.ts
✔ Generate types for contract ABIs
✔ Generate types for data source templates
✔ Load data source template ABIs
✔ Generate types for data source template ABIs
✔ Load GraphQL schema from schema.graphql
  Write types to generated/schema.ts
✔ Generate types for GraphQL schema

Types generated successfully

  Skip migration: Bump mapping apiVersion from 0.0.1 to 0.0.2
  Skip migration: Bump mapping apiVersion from 0.0.2 to 0.0.3
  Skip migration: Bump mapping apiVersion from 0.0.3 to 0.0.4
  Skip migration: Bump mapping apiVersion from 0.0.4 to 0.0.5
  Skip migration: Bump mapping apiVersion from 0.0.5 to 0.0.6
  Skip migration: Bump manifest specVersion from 0.0.1 to 0.0.2
  Skip migration: Bump manifest specVersion from 0.0.2 to 0.0.4
✔ Apply migrations
✔ Load subgraph from subgraph.yaml
  Compile data source: OnePieceMint => build/OnePieceMint/OnePieceMint.wasm
✔ Compile subgraph
  Copy schema file build/schema.graphql
  Write subgraph file build/OnePieceMint/abis/OnePieceMint.json
  Write subgraph manifest build/subgraph.yaml
✔ Write compiled subgraph to build/

Build completed: build/subgraph.yaml

graph deploy --studio onepiece

Which version label to use? (e.g. "v0.0.1"): v0.0.1
  Skip migration: Bump mapping apiVersion from 0.0.1 to 0.0.2
  Skip migration: Bump mapping apiVersion from 0.0.2 to 0.0.3
  Skip migration: Bump mapping apiVersion from 0.0.3 to 0.0.4
  Skip migration: Bump mapping apiVersion from 0.0.4 to 0.0.5
  Skip migration: Bump mapping apiVersion from 0.0.5 to 0.0.6
  Skip migration: Bump manifest specVersion from 0.0.1 to 0.0.2
  Skip migration: Bump manifest specVersion from 0.0.2 to 0.0.4
✔ Apply migrations
✔ Load subgraph from subgraph.yaml
  Compile data source: OnePieceMint => build/OnePieceMint/OnePieceMint.wasm
✔ Compile subgraph
  Copy schema file build/schema.graphql
  Write subgraph file build/OnePieceMint/abis/OnePieceMint.json
  Write subgraph manifest build/subgraph.yaml
✔ Write compiled subgraph to build/
  Add file to IPFS build/schema.graphql
                .. Qmb6bsS1CY1PnbPRrJNGavfCfibqSz9TrRNGVFwtUT6EBL
  Add file to IPFS build/OnePieceMint/abis/OnePieceMint.json
                .. QmRb3G7FHkZ4jB9uxS5ypUY924iD9kiGwsVJ1r5sd7dyDJ
  Add file to IPFS build/OnePieceMint/OnePieceMint.wasm
                .. QmXmz7beDyecgERBMLCihi3GxdebYvXo3JjrDet79tHsok
✔ Upload subgraph to IPFS

Build completed: QmPV1dgcrkBrmcMgPWegzN5G1dso5RPEfvhuGsdyPKCnbf

Deployed to https://thegraph.com/studio/subgraph/onepiece

Subgraph endpoints:
Queries (HTTP):     https://api.studio.thegraph.com/query/68007/onepiece/v0.0.1

```

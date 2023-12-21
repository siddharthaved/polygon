# Polygon Assessment

## Space ERC 721A NFT Collection bridge from Etherium Goerli to Polygon Mumbai network  

This repository contains a Solidity smart contract for Space NFTs (Non-Fungible Tokens). The contract is built using the ERC721 standard and extends the functionality with ERC721A, which supports batch minting.
### Requirements 

- Node.js and npm should be installed on your machine.
- Create a `.env` file and set the `PRIVATE_KEY` and other necessary environment variables.
  
## Contract Details

- Contract Name: Space
- Symbol: Spc
- Base URL for NFTs: "https://gateway.pinata.cloud/ipfs/QmUHVj7XKfSsjBfzfcnxhfY2C8hv7pvABWxbZ3WwT3EG9N/"
- Prompt: "robots reading Sanskrit scripts in outer space to restore Earth"
  

## Smart Contract Details

The smart contract has the following features:

- Batch minting of NFTs: The contract allows the owner to mint a specified number of Space NFTs in a single transaction using the `mint` function.

- Ownership: The contract inherits from the OpenZeppelin Ownable contract, allowing only the contract owner to mint NFTs.

- Base URI: The `_baseURI` function is overridden to set the base URL for the generated NFTs.

## Deployment

To deploy the Space NFT contract, use the following script:

```bash
npx hardhat run scripts/deploySpace.js --network <NETWORK_NAME>
```

## Minting NFTs

To mint Space NFTs using the deployed contract, use the following script:

```bash
npx hardhat run scripts/mintNFTs.js --network <NETWORK_NAME>
```

## Deposit NFTs to FxChain

To transfer ERC721A tokens (Space NFTs) to the Ethereum FxChain network, use the following script:

```bash
npx hardhat run scripts/depositNFTsToFxChain.js --network <NETWORK_NAME>
```

Note: Replace `<NETWORK_NAME>` with the desired network (e.g., "goerli", "rinkeby", etc.).



## License

This project is licensed under the MIT License. See the `LICENSE` file for more details.



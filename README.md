# Eigenlayer Beacon Oracle

This repository contains the smart contract for the Eigenlayer Beacon Oracle. It uses the beacon roots precompile added in [EIP-4788](https://eips.ethereum.org/EIPS/eip-4788) to find the block root for a given timestamp.

## Sepolia Deployment

Currently, the Eigenlayer Beacon Oracle is deployed on Sepolia [here](https://sepolia.etherscan.io/address/0x2b3F237861C5e76e43e9a7a597a3a364d2D5C58e).

### Deploy

To deploy the contract on a chain, run the following command:

```shell
$ cd contracts
$ forge script script/DeployEigenLayerBeaconOracle.s.sol:DeployEigenLayerBeaconOracle --rpc-url <your_rpc_url> --private-key <your_private_key>
```

### Run Script

To run the script which periodically updates the oracle, run the following command:

```shell
$ cargo run --release
```

Make sure to set the enviroment variables in `.env` before running the script.
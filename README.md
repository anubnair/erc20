# ERC20
sample erc20 contract

## Installed Lib
https://github.com/foundry-rs/forge-std/tree/v1.7.1
https://github.com/OpenZeppelin/openzeppelin-contracts/tree/v5.0.0

## How to install packages?
forge install OpenZeppelin/openzeppelin-contracts

## How to deploy contract?
FOUNDRY_PROFILE=fuji forge create \
--mnemonic .mnemonic \
--from 0xA481a2A16C09c60472967ceD59e3d4d6C799F5E8 \
--legacy \
src/MyToken.sol:MyToken

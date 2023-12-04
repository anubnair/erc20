# ERC20
sample erc20 contract

## Installed Lib
https://github.com/foundry-rs/forge-std/tree/v1.7.1
https://github.com/OpenZeppelin/openzeppelin-contracts/tree/v5.0.0

## How to install packages?
forge install OpenZeppelin/openzeppelin-contracts
forge install foundry-rs/forge-std

## How to deploy contract?
FOUNDRY_PROFILE=fuji forge create \
--mnemonic .mnemonic \
--from 0xA481a2A16C09c60472967ceD59e3d4d6C799F5E8 \
--legacy \
src/MyToken.sol:MyToken

=======

Deployment in Neon:

FOUNDRY_PROFILE=neon-devnet forge create \
--mnemonic .mnemonic \
--from 0xA481a2A16C09c60472967ceD59e3d4d6C799F5E8 \
--legacy \
src/MyToken.sol:MyToken

Deployed to: 0xdAc6f3057836b7e6688CA5Ae17F6e13fADb9924c
Transaction hash: 0x26633de040ed2f7ca6ab7b7b12b7310fe6c682c0641187a69ff5e8a750601661


Deployment in Polygon mumbai:

FOUNDRY_PROFILE=polygon-mumbai forge create \
--mnemonic .mnemonic \
--from 0xA481a2A16C09c60472967ceD59e3d4d6C799F5E8 \
--legacy \
src/MyToken.sol:MyToken

Deployer: 0xA481a2A16C09c60472967ceD59e3d4d6C799F5E8
Deployed to: 0xf461ba7cfdFdEf7c3E887144CAcE8D944C4381A4
Transaction hash: 0x71abbbb37698ffb6ecc019e8e93c99886ca0a31a01ff5be954b35bd54c604866



## check balanceOf
====
FOUNDRY_PROFILE=neon-devnet cast call \
0xdAc6f3057836b7e6688CA5Ae17F6e13fADb9924c \
"balanceOf(address)" 0xa481a2a16c09c60472967ced59e3d4d6c799f5e8

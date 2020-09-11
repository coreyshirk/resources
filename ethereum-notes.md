# Ethereum Notes

## Ethereum Accounts
Account consists of three pieces:
- Account Address (unique identifer to share)
- Public Key
- Private Key

The combination of the public and private key are used to sign transactations.


## Ethereum Blocks
When a valid block is found, the block is broadcasted with:
- Transaction list
- Uncle list
- Block header:
  - Previous block hash
  - State root
  - Transactions root
  - Reciepts root
  - Block number
  - Gas used
  - Timestamp
  - Nonce

## Solidity
Developers write Ethereum Contract Definitions with Solidity, the Solidity Compiler spits out Bytecode and ABI (Application Binary Interface). The Bytecode is deployed to the Ethereum blockchain and ABI is the interface for the contract's Bytecode.

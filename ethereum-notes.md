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
Developers write Ethereum Contract Definitions with Solidity, the Solidity Compiler spits out Bytecode and ABI (Application Binary Interface). The Bytecode is deployed to the Ethereum blockchain and the ABI is the interface for the contract's Bytecode.

### Running Contract Functions
| "Calling" a function | Sending a Transaction to a Function |
|------------------------------------|-------------------------------|
| Cannot modify the contract's data  | Can modify the contract data  |
| Can return data                    | Takes time to execute         |
| Runs instantly                     | Returns the transaction hash  |
| Free to do.                        | Costs gas(ETH)!               |

Anytime that a transaction is submitted to the network it takes time to process. (15-30 seconds to execute)
When sending a transaction to a function it returns the transaction hash (identifies the transaction that occurs).
Sending a transaction to a function cost gas.



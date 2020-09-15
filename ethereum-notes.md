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
## Ethereum Denominations
| Unit                    | Wei Value | Wei                                       |
|-------------------------|-----------|-------------------------------------------|
| **wei**                 | 1 wei     | 1                                         |
| **Kwei (babbage)**      | 1e3 wei   | 1,000                                     |
| **Mwei (lovelace)**     | 1e6 wei   | 1,000,000                                 |
| **Gwei (shannon)**      | 1e9 wei   | 1,000,000,000                             |
| **microether (szabo)**  | 1e12 wei  | 1,000,000,000,000                         |
| **milliether (finney)** | 1e15 wei  | 1,000,000,000,000,000                     |
| **ether**               | 1e18 wei  | 1,000,000,000,000,000,000                 |


## Solidity
Developers write Ethereum Contract Definitions with Solidity, the Solidity Compiler spits out Bytecode and ABI (Application Binary Interface). The Bytecode is deployed to the Ethereum blockchain and the ABI is the interface for the contract's Bytecode. The ABI connects the Solidity world to our programming lanugage (Javascript, Python, etc...).

### Running Contract Functions
| "Calling" a function | Sending a Transaction to a Function |
|------------------------------------|-------------------------------|
| Cannot modify the contract's data  | Can modify the contract data  |
| Can return data                    | Takes time to execute         |
| Runs instantly                     | Returns the transaction hash  |
| Free to do.                        | Costs gas(ETH/Wei)!               |

- Anytime that a transaction is submitted to the network it takes time to process. (15-30 seconds to execute)
- When sending a transaction to a function it returns the transaction hash (identifies the transaction that occurs).
- Sending a transaction to a function cost gas.

### Gas and Transactions
|Term | Definition |
|-----|------------|
|gasPrice | Amount of Wei the sender is willing to per unit of gas to get this transaction processed |
|startGas/gasLimit | Units of gas that this transaction can consume |

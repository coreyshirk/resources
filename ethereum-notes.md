# Ethereum Notes

Account consists of three pieces:
- Account Address (unique identifer to share)
- Public Key
- Private Key

The combination of the public and private key are used to sign transactations.


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

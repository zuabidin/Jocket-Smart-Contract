# Jockey Smart Contract
Random Number Generator on Blockchain

This is a Smart Contract written in Solidity which tackles the problem of generating a random number on Blockchain. Out of various approaches it uses the approach below:

# Approach
Blockhash of a future block
 * A better approach is to use the blockhash of some future block. The implementation scenario is as follows:
  1. The player makes a bet and the house stores the block.number of the transaction.
  2. In a second call to the contract, the player requests that the house announces the winning number.
  3. The house retrieves the saved block.number from storage and gets its blockhash, which is then used to generate a pseudo-random number.

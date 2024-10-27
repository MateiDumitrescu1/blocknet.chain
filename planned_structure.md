# Components of blockchains in general  
## Block
## Blockchain
The blockchain is essentially a list (or chain) of blocks. It manages:  
Chain Integrity: Ensuring blocks are linked correctly.   
Consensus Mechanism: Agreeing on the current state among nodes.   
Adding New Blocks: Validating and appending new blocks.   
## Node
## P2P Network  
## Consensus Algorithm  
A consensus algorithm ensures all nodes agree on the blockchain's state.  
Ensures: secure and transparent transaction recording 
Ensures: transactions added to blockchain are legitimate
https://www.geeksforgeeks.org/consensus-algorithms-in-blockchain/  
#### Proof of Work (PoW)
Requires network participants to solve computational problem, requiring a lot of compute. Reward: participants gets to add the next block to the chain and gets some ammount of currency
#### Proof of Stake (PoS)
Aims to solve the energy consumption and compute problems of PoW.  
Network participants are required to stake a certain amount of cryptocurency in the network. Then the network randomly selects a participants (called a validator) to validate the new block, collect some fees from the transactions of that block or some native tokens of the network they validate. This way, **validators** are rewarded for the helping the consensus of the network.    

By receiving rewards, **validators** are incentivized to act honestly and in the network's best interest. Any malicious behavior or negligence may result in penalties, slashing of rewards, or loss of their stake.  
**Validators** are crucial to PoS. Becoming a **validator** means meeting certain requirements (like minimum amount of coins staked). Once selected, **validators** perform tasks such as verifying transactions, checking the validity of blocks, and proposing new blocks for inclusion in the blockchain.   
How proposing new blocks works: every 10s (for example), the chosen **validator** selects pending transactions in the transaction pool (sometimes called **mempool**) and organizez them into a block. The **validator** then broadcasts the block to the network.  


#### Dedicated Proof of State (DPoS)
https://www.ledger.com/academy/what-is-delegated-proof-of-stake-dpos  
Network users vote and elect **delegates** to validate the next block.  
Users vote for a certain **delegate** by pooling their tokens into a staking pool and linking those the delegate. The delegate with the most tokens may then validate a block, and receive the corresponding transaction fees as a reward. Next, the delegate distributes the rewards to users who supported them based on each user’s stake.  

Users can also vote out delegates if they make malicious attempts on the network. As such, delegates with a strong reputation are usually elected as witnesses.  
# Components of blocknet  

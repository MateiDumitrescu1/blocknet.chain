# Block
https://www.investopedia.com/terms/b/block-bitcoin-block.asp#:~:text=Blocks%20are%20files%20stored%20by,be%20entered%20into%20and%20validated.

Blocks store files that are hashed and encode into a Merkle Tree. Once the data is validated, the block is closed.      
A block is thus a permanent store of records that, once written, cannot be altered or removed without changing all preceding or   following blocks.     
### Blocksize    
Set the size so there is a limit to how much information can be written   
### Block header  
Contains information about the block 
#### Previous block hash
#### Timestamp
#### Merkle Tree Hash
#### Difficulty Target
how difficult the block hash is ?????
#### Nonce
32-bit number assigned to the block in the mining process, that is incremented by 1 every time a guess is made.
### Content
The content 

# Blockchain
The blockchain is essentially a list (or chain) of blocks. It manages:  
Chain Integrity: Ensuring blocks are linked correctly.   
Consensus Mechanism: Agreeing on the current state among nodes.   
Adding New Blocks: Validating and appending new blocks.   
# Node
# P2P Network  
# Consensus Algorithm  
A consensus algorithm ensures all nodes agree on the blockchain's state.  
Ensures: secure and transparent transaction recording 
Ensures: transactions added to blockchain are legitimate
https://www.geeksforgeeks.org/consensus-algorithms-in-blockchain/  
### Proof of Work (PoW)
Requires network participants to solve computational problem, requiring a lot of compute. Reward: participants gets to add the next block to the chain and gets some ammount of currency
### Proof of Stake (PoS)
Aims to solve the energy consumption and compute problems of PoW.  
Network participants are required to stake a certain amount of cryptocurency in the network. Then the network randomly selects a participants (called a validator) to validate the new block, collect some fees from the transactions of that block or some native tokens of the network they validate. This way, **validators** are rewarded for the helping the consensus of the network.    

By receiving rewards, **validators** are incentivized to act honestly and in the network's best interest. Any malicious behavior or negligence may result in penalties, slashing of rewards, or loss of their stake.  
**Validators** are crucial to PoS. Becoming a **validator** means meeting certain requirements (like minimum amount of coins staked). Once selected, **validators** perform tasks such as verifying transactions, checking the validity of blocks, and proposing new blocks for inclusion in the blockchain.   
How proposing new blocks works: every 10s (for example), the chosen **validator** selects pending transactions in the transaction pool (sometimes called **mempool**) and organizez them into a block. The **validator** then broadcasts the block to the network.  


### Dedicated Proof of State (DPoS)
https://www.ledger.com/academy/what-is-delegated-proof-of-stake-dpos  
Network users vote and elect **delegates** to validate the next block.  
Users vote for a certain **delegate** by pooling their tokens into a staking pool and linking those the delegate. The delegate with the most tokens may then validate a block, and receive the corresponding transaction fees as a reward. Next, the delegate distributes the rewards to users who supported them based on each user’s stake.  

Users can also vote out delegates if they make malicious attempts on the network. As such, delegates with a strong reputation are usually elected as witnesses.    
### Leased Proof of State (LPoS)   
https://www.lcx.com/leased-proof-of-stake-lpos-explained/#:~:text=LPoS%20is%20a%20proof%2Dof,of%2Dstake%20(DPoS).    
1. `Create a lease transaction`: Tokenholders lease coins to a node by specifying the quantity and recipient address in a lease transaction. Any lease can be terminated at any time.  
2. `Wait for block generation`: Leased funds are added to a node’s pool, enhancing the likelihood of winning the next block’s lottery.  

### Proof Of Authority (PoA)   
private or consortium blockchain  
validators are some established trusted nodes. This sacrifices decentralization   

### Byzantine Fault Tolerance (BFT)
https://medium.com/@abhilashkrish/byzantine-fault-tolerance-bft-consensus-4f214c49f07d  
Designed to tolerate fraud    
BFT is the ability of a distributed network to function as desired and correctly reach a sufficient consensus despite malicious nodes that propagate false information to peers.  

#### Practical Byzantine Fault Tolerance (P-BFT)   
Consensus is reached is 2/3 of nodes agree on a transaction. If a malicoious party controls more than 1/3 of nodes, then they can compromise the network.  

#### Dedicated  Byzantine Fault Tolerance (D-BFT)  
Nodes are assigned to groups, each group has a designated leader (called delegate). Leaders are repponsible for proposing new blocks, the rest of nodes in the group validate the proposed block.
D-BFT is faster and more efficient than P-BFT.  

### DAG 

 #Eth #Mev #secruity 
 


# What is MEV

Maximal extractable value  

- A value that can be extracted by recording including or censoring a transaction. 
- The way transactions are processed in the blockchain.

flowchart LR

```mermaid 
sequenceDiagram
    participant User
    participant Mempool
    participant Searcher
    participant Validator
    participant Blockchain

    User->>Mempool: Sends a Transaction (e.g., Swap on Uniswap)
    Searcher->>Mempool: Scans for profitable TXs
    Searcher->>Searcher: Inserts their TX (e.g., Sandwich Attack)
    Searcher->>Validator: Pays high gas to prioritize order
    Validator->>Blockchain: Mines Block
    Blockchain->>Searcher: Profit realized from MEV extraction
```

# MEV Sandwich Attack

```mermaid
sequenceDiagram
    participant Victim
    participant Attacker
    participant DEX
    participant Blockchain

    Victim->>DEX: Buy Token X
    Attacker->>DEX: Front-runs (Buys before Victim)
    DEX->>Blockchain: Process Order
    Victim->>Blockchain: Executes Trade at Worse Price
    Attacker->>DEX: Back-runs (Sells at inflated price)
    Attacker->>Blockchain: Profits from the spread

```

j
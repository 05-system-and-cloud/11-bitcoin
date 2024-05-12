## 1. What is Bitcoin?

- Bitcoin is `an electronic payment system` that allows anyone to `create an account` and `send any amount of money to anyone` in the world
- It was created as `an alternative` to the current financial system which `centralizes the control of money`, and we have no other option but to trust these banks to act fairly and responsibly.

## 2. How Bitcoin work?

- Bitcoin is just `a computer program` and `connect to other computers` running the same program, and they will start `sharing a file` with you
- When a new transaction enters the network, it gets `relayed from computer to computer` until `everyone has a copy` of the transaction
- At roughly `10 minute intervals`, `a random computer (node)` on the network will `add the latest transactions they have received` on `to the blockchain`, and `share the updates` with everyone else
- As a result, `a large network of computers` that `communicate with each other` to `share a file and update it` with new transactions

## 3. What problem does Bitcoin solve?

- Bitcoin solves the problem of being able to have `a payment system that operates without a central point of control` (decentralized)
- Bitcoin solves the `double-spend (two separate transactions for the same coin)` problem by `forcing nodes` to `keep all the transactions they receive in memory` before writing them to a file. Then, `at 10-minute intervals`, `a random node` on the network `will add the transactions from their memory` on to the file.
- This updated file is then `shared with the rest` of the network. Nodes will `accept the transactions in the updated file` as the "correct" ones, and `remove any conflicting transactions from their memory`

## 4. How does mining work?

- Mining is the process of `adding new blocks of transactions` on to the blockchain
- To do `mining`, a node will `gather the transactions` from `its memory pool (temporary memory on their computer)` in to `a container called a block`, and then use `processing power` to try and `add this block of transactions on to the blockchain`
- Processing power is the process for `adding block of transactions` in to something called `a hash function` which take in any `amount of data`, `scramble it`, and spit out `a completely unique (and unpredictable) number`
- So in summary, the process of mining uses processing power to `perform hash calculations` as fast as you can to try and `be the first computer` on the network to `get a block hash below the target (threshold that everyone on the network agrees upon)`. If you're successful, you can `add your block of transactions on to the blockchain` and `share it with the rest` of the network.

## 5. Why is the file called the "blockchain"?

- Transactions are not added to the file individually – they are `collected together and added in blocks`. Each of these `new blocks builds on top of an existing one`, and so the file `is made up of a chain of blocks`; hence, blockchain.
- Miners will always try to `build on top of the "tip" of the longest known chain of blocks`, as any transactions that `are not part of the longest chain` will be `invalid`
- Therefore, if someone wanted to rewrite the history of transactions, they would need to `rebuild a longer chain of blocks` to `create a new longest chain` for other nodes to adopt. However, to achieve this, a single miner would `need to have more computer processing power than the rest` of the network combined

## 6. How do transactions work?

- Blockchain is consider as a storage facility for `safe deposit boxes`, which we call `outputs (a package of bitcoins)`. These outputs are just `containers that hold various amounts of bitcoin`
- When you send bitcoins to someone , you are actually `placing an amount of bitcoins from your selecting existing outputs (that you can unlock)` in to `a new safe deposit box (new output)`, and `putting a lock on it` that `only the person you are "sending"` the bitcoins to `can unlock`

## 7. How do you own bitcoins?

- To be able to receive bitcoins, you need to `have your own set of keys (public key and private key)`
- If I want to send bitcoins to you
  . You need to `give me your the public key`
  . When I create a transaction, I would `place your public key inside the lock on the output` (the safe deposit box)
  . And when you want use these bitcoins (send to someone else), you would `use your private key to unlock this output`

- In short, your `private key is just a large random number`, and your `public key is a number calculated from this private key`
- When you want to `unlock bitcoins` that are `assigned to your public key`, you `use your private key to create` what's called a `digital signature`
- This signature proves that `you are the owner of the public key`, without having to reveal your private key
- This signature is also `only valid for the transaction it was created for`, so it cannot be used to unlock other bitcoins locked to the same public key

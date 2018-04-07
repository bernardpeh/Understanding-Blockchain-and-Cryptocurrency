# Cryptocurrency

The features of the blockchain technology makes it a good candidate for currency creation. Cryptocurrency (aka crypto) = digital currency secured by cryptography. In short, it means a digital currency that allows transfer of value and does not allow double spending.

“Announcing the first release of Bitcoin, a new electronic cash system that uses a peer-to-peer network to prevent double-spending. It’s completely decentralized with no server or central authority.”  – Satoshi Nakamoto, 09 January 2009

Today, we have thousands of cryptocurrencies. The top cryptocurrencies can be found in [https://coinmarketcap.com/](https://coinmarketcap.com/) (CMC)

Bitcoin (BTC), Ethereum (ETH) and Ripple (XRP) are the top 3 most popular crypto at the time of writing.

## How can I get Cryptocurrencies?

* Mine: Some coins such as bitcoin and ethereum can be mined. Bitcoin can be mined (solving mathematical puzzles) using CPU, graphics card or specialised machine known as ASICS. Ethereum on the other hand can be mined with cpu or graphics card.

* Buy/Trade: The easiest way to get some crypto is to buy it using fiat or trade it with other crypto in crypto exchanges. Some popular exchanges are https://coinbase.com, https://www.bitfinex.com, https://bittrex.com, https://btcmarkets.net (Aussie) and many others. It is also possible to buy or trade crypto with friends or trusted individuals.

* Stake: Some coin such as NEO rewards people by just holding onto it. Think of it like a term deposit.

## How does Crypto Mining work?

When a miner (machine) is doing crypto mining (aka Proof of Work or POW), it is actually trying to assemble all the transactions in the network into a block. The first miner that does it correctly and acknowledged by the network will be rewarded with some coins. Take bitcoin for example, it has block size limit of 1 MB at the time of writing. If each transaction has a size of 226 bytes, this means a block can include a maximum of 4500 transactions. If each block generation is 10 mins, this gives a rate of 7.5 txs/sec (a number we are lucky to have).

Check out the latest blocks mined at [https://blockchain.info/blocks](https://blockchain.info/blocks )

What if bitcoin becomes really popular and everyone starts using it? The 7 txs/sec limit wouldn’t able to accomodate the heavy traffic. This is where it gets tricky and hence the reason why we need to understand how the miner software operates.

When we send some bitcoin to someone, we set the transaction fee to use per byte. The miner doesn’t work on the first come first serve basis, but rather gives priority to the transaction that comes with a higher transaction fee. So it is possible for your transaction to be processed really slowly or get “Stuck” and not be processed at all if your transaction fee is too low. With the price of bitcoin today, recommended transaction fees can sometimes go as high as 30 - 80 USD.

Knowing how mining and transaction fee works is important when you trade POW coins.

## Different types of Crypto Wallet

* A crypto wallet is a software or hardware that stores your private keys. Each wallet can have many crypto accounts and each account is simply the public key generated from the private key, ie a hexadecimal address. Different cryptocurrency uses different blockchain and hence, have different address format. You will send and receive crypto to and from an address.

* Online Wallet: These are wallets that you access via your web browser. It includes all the wallets in any websites and exchanges. Examples are blockchain.info, exchanges wallet.
Software Wallet: These are mobile or desktop software wallets. Examples are Jaxx, Electrum, BreadWallet, Mycelium, and CoPay.

* Hardware Wallet: These are actual hardware devices. All private keys never leave the devices. They are usually clunkier and less user friendly than the web wallets. Trezor and Ledger are popular hardware wallets.

* Paper Wallet: You write down your private key on paper and have to type in the keys manually when sending funds. This is a good option if you do not intend to use your crypto for a long time.

* Multisig Wallet: A wallet that can only send funds when approved by “X” key holders.
We recommend using hardware wallet at all times and only transfer quantities you need to the crypto exchange as and when you need it.

## Centralised VS Decentralised Exchanges

An exchange is a marketplace where crypto assets are traded. 

The largest stock exchange in the world, ie New York Stock Exchange is centralised. **A centralised exchange means all trading happens within the exchange own account almost instantaneously.** A buy and sell order for example is off-chain, ie a simple database insert or update. Trading is quick because it doesn’t need to go through the blockchain and wait for transaction confirmation. Most crypto exchanges at the moment are centralised. The downside is that your crypto is stored in the exchange wallet and you must trust them with it. If the exchange is hacked, you will lose your crypto as well. Simple googling will reveal many high profile centralised exchanges being hacked.

A decentralized exchange does not hold customer's funds. Trading occurs on-chain directly between users through a smart contract or proxy tokens or other solutions. The immediate benefit is that your crypto is held in the smart contract, not the exchange wallet until after the trading is done. However, there are [a lot more problems](http://hackingdistributed.com/2017/08/13/cost-of-decent/) that come with decentralised exchange at the time of writing. Trading is also slow and clunky as it is real time and on-chain. An example of a popular Ethereum decentralised exchange is https://etherdelta.com. However, off-chain technologies like the [Lightning Network](https://lightning.network/) will make decentralised exchange possible

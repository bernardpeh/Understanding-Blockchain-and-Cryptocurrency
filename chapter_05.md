# Ethereum

## The Ethereum Virtual Machine

In the Ethereum blockchain, each transaction is not just a value transfer, it can consist of instructions to interact with any Smart Contract that lives in the chain, including deploying Smart Contracts.

EVM is like a runtime operating system that executes the Smart Contract. Each node running the Ethereum client will also run the EVM. EVM is also turing complete, meaning it could perform any logic operations such as running a never ending loop.

## Transaction Fee

Gas in Ethereum is like tx fee in Bitcoin. 

Unlike Bitcoin, Ethereum allows endless loops in a Smart Contract. Hence, there is a need to discourage malicious Smart Contract from looping forever and jamming the node and the network.

Every computation step will cost “Gas” and if the gas limit is reached, the Smart Contract instruction will not be executed and the transaction fee penalised.

User will need to specify the gas limit and gas price before sending ETH.

**Transaction Fee = Gas x Gas Price**

## ERC20 Token

[ERC20](https://en.wikipedia.org/wiki/ERC20) is the standard for creating currency (Token) within the Ethereum blockchain. There are ways to create tokens in other blockchains but Ethereum ERC20 is by far the most popular way at the time of writing. For those who are familiar with computer programming, think of it like an interface where certain methods must be implemented.

## ICO

[ICO](https://blockgeeks.com/guides/initial-coin-offering/) (Initial Coin Offerings) is an excellent way to fund projects by rewarding tokens/coins to its contributors. Many ICOs use the Ethereum ERC20 token as a currency. The idea is that you send some crypto to an address and in return, the ICO company will send you x number of tokens (based on certain exchange rate) to an Ether address that you specify. The token itself is a cryptocurrency and will have more monetary value as the project becomes more successful. Many top tokens in https://coinmarketcap.com are ERC20 Tokens. Many people like to invest in ICO simply because they believe in the monetary value of the token when it hits major crypto exchanges.

Indeed, ICO is putting kickstarter to shame since 2014 because of the [sheer amount of money](http://www.businessinsider.com/biggest-cryptocurrency-ico-ever-going-on-right-now-2017-12/?r=AU&IR=T) it can raise. Unfortunately, it is also a target for scammers.

ICO can be ran **manually** or automated using a **Smart Contract**. There are pros and cons for each method. 

**In the manual method, you sent the crypto directly to a user address** and there is a human or scheduler in the server backend to process the payment and assign you the credit in their database. Once the ICO is over, you have to specify an Ethereum address to be credited and the company will send you the ERC20 token manually. The main benefit of the manual method is simplicity in implementation, ie your Smart Contract contains very little logic. There is one big problem however and that is there is no transparency in the process and you have to trust the company to pay you the token at the end. You also do not know how much is being raised during the ICO because there is no Smart Contract to verify against.  

**When using the Smart Contract method, you send Ether to the Smart Contract** and it will credit you immediately with the ICO token based on certain exchange rate as determined in the contract. (A Smart Contract in Ethereum is just like any other user address with code that can be examined by everyone). 3 information must be provided, ie contribution address, gas limit and gas price. Unlike sending ETH to a user account, the gas limit for an ICO smart contract is usually much higher, around 250000. When sending the Ether, It doesn’t matter if the contract actually consumes much lesser gas because the unused gas will be returned to you. In simple terms, there is no harm putting a higher gas limit. The only exception is if the contract is faulty, it might consume all your gas and you lose your transaction fee.

If you are sending ETH directly to a Smart Contract, you should not do so from an exchange address because the sender address (in this case, is the exchange wallet not your personal wallet) will be usually credited with the token instead.

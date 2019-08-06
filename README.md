# Lottery.sol
A lottery smart contract in Solidity

This lottery contract allows anyone to buy a ticket at a set price, and draws two winners.

We first built a very simple Raffle contract to which anyone can enter by paying for their ticket. We allowed anyone to draw a random winner at any time.

Then we started from scratch, building a lottery smart contract which picked two winners. This was purposefully complicated. After enough players entered, the competition was closed and two draws took place. The first winner had to be removed from the second lottery round and the winnings had to be split equally. To make it safe, we had to generate truly random numbers, which is difficult on Ethereum.

Only one ticket can be issued per address. Anyone can call the draw function, after which a random winner is chosen. The draw function can then be called again for the second winner. The bounty is split in half for each winner. After two winners are chosen, the contract destructs.

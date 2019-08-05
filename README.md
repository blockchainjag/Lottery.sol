# Lottery.sol
A lottery smart contract in Solidity

This lottery contract allows anyone to buy a ticket at a set price, and draws two winners.
Only one ticket can be issued per address. Anyone can call the draw function, after which a random winner is chosen. The draw function can then be called again for the second winner. The bounty is split in half for each winner. After two winners are chosen, the contract destructs.

# MyToken

This is a simple solidity contract which creates and destroys the tokens along with stores some information about the tokens.

## Description

This program is a simple contract written in Solidity, a programming language used for developing smart contracts on the Ethereum blockchain. The contract has two functions called MINT and BURN which will increase and decrease the balance amount.

## Requirements

1. The contract has public variables that stores details about the coin:
   -'TokenName':This string gives the name of the token.
   -'TokenAbbrv':This string gives the abbreviation the token.
   -'TotalSupply':This is an unsigned integer which gives total supply of token and it initially has value 0.

2. The contract has a mapping of addresses to balances(address => uint):
   -'balances': A mapping that maps addresses with their corresponding token balances.

3. The contract has a 'mint' function that increases the total supply and the balance of the "sender" address by a given value:
   - Parameters:
     - 'Address': The address to which the tokens will be minted.
     - 'Value': The amount of tokens to be minted.
   - Actions:
     - Increase the 'TotalSupply' by 'Value'.
     - Increase the balance of that 'Address' by 'Value'.

  4.The contract has a 'burn' function that decreases the total supply and the balance of the "sender" address by a given value:
   - Parameters:
     - 'Address': The address from which the tokens will be burned.
     - 'Value': The amount of tokens to be burned.
   - Actions:
     - Check if the balance of the 'Address' is greater than or equal to 'Value'.
     - If it is true, decrease the 'TotalSupply' by 'Value'.
     - Decrease the balance of the 'Address' by 'Value'.
    
### Deploying

1. Deploy the 'MyToken' contract in Remix,an online solidity IDE.

2. Once deployed, you can interact with the contract by calling the above functions,you can change values to check whether your contract is working correctly.

## License

This contract is licensed under the MIT License. SPDX-License-Identifier: MIT.


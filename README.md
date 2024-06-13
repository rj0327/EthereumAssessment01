MyToken Smart Contract
This Solidity program defines a simple token contract named "ROHAN" with the symbol "RJ". It allows minting and burning of tokens, tracking balances for different addresses.

Requirements
Public Variables:

tokenname: Stores the name of the token ("ROHAN").
tokenabbrv: Stores the abbreviated symbol of the token ("RJ").
totalSupply: Tracks the total supply of tokens.
Mapping:

Balance: Maps addresses to their respective token balances.
Mint Function:

Increases the total supply and the balance of a specified address.
Burn Function:

Decreases the total supply and the balance of a specified address, if the balance is sufficient.
Usage
Mint Tokens:

Call mint(address _address, uint _value) to add tokens to an address.
Burn Tokens:

Call burn(address _address, uint _value) to remove tokens from an address, ensuring the balance is sufficient.

Deployment
Deploy the contract using a Solidity development environment like Remix. Once deployed, interact with the contract by calling mint and burn functions to manage token balances.

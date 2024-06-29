**#MyToken Smart Contract**

A basic Solidity smart contract for a token called "ROHAN" with the symbol "RJ" can be found in this repository. The contract maintains balances for various addresses and permits token minting and burning.

## Contract Information

- **Token Abbrevation**: ROHAN
- **Token Name**: RJ
- **Total Supply**: Starting at 0

## Features

- Minting tokens: Adds more tokens to the total supply and credits the designated address with them.
- Burning tokens: If the address has enough tokens, this reduces the total supply and debits the designated address.

## Functions

### Open Variables

- {string public tokenName}: The token's name.
- {string public tokenAbbrv}: The token's Abbreviation.
- {uint public totalSupply}: The token's total supply.

### Mapping

 mapping that maintains track of the balance for each address is mapping(address => uint) public Balance.
### Mint Function - 

Tokens can be created and assigned to a specific address using the mint function. As a result, the recipient address's balance and the total number of tokens available increase.

### Burn Function: 

Using the burn function, tokens from a given address can be destroyed. Assuming the holder has sufficient tokens to burn, this reduces both the total supply of tokens and the balance in their address.

# Interacting with the Contract
You can interact with the deployed contract using Ethereum wallets or by writing scripts in programming languages like JavaScript. Here's how you can interact with the contract:

Minting Tokens: Call the mint function with the address where you want to send the tokens and the amount to mint.
Burning Tokens: Call the burn function with the address from where you want to burn the tokens and the amount to burn.


### Executing Program

#### How to Run the Program in Remix
1. **Compile the Smart Contract**
   - Select the `Solidity Compiler` tab.
   - Ensure the compiler version is set to `0.8.18`.
   - Click `Compile MyToken.sol`.

2. **Deploy the Contract**
   - Go to the `Deploy & Run Transactions` tab.
   - Select the appropriate environment (e.g., JavaScript VM).
   - Click `Deploy`.

3. **Interact with the Contract**
   - After deploying, the contract will appear under `Deployed Contracts`.
   - To mint tokens:
     - Input the address and the amount of tokens to mint.
     - Click the `mint` button.
   - To burn tokens:
     - Input the address and the amount of tokens to burn.
     - Click the `burn` button.

## Author

Name - [Rohan Jha](rj0327)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.


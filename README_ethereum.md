# MyToken Smart Contract

This Solidity program defines a simple token contract named "ROHAN" with the symbol "RJ". It allows minting and burning of tokens, tracking balances for different addresses.

## Description

The "ROHAN" token contract is a basic implementation of a token system using Solidity. The contract supports minting and burning of tokens, allowing users to increase or decrease the total supply of tokens. Each address holds a balance that can be updated through these operations. The contract is ideal for learning and simple applications where a basic token system is required.


## Getting Started

### Installing

* How/where to download your program
Download and interact with the contract using a Solidity development environment like Remix. You can access Remix here.
* Any modifications needed to be made to files/folders
No specific file or folder modifications are needed. Ensure your Solidity environment is set up correctly to compile and deploy contracts.



### Executing program

* How to run the program
* To deploy and interact with the contract, follow these steps:

1. Open Remix at Remix Ethereum.
2. Create a new file and paste the Solidity code for the MyToken contract.
3. Compile the contract by selecting the correct compiler version (0.8.26) and clicking "Compile".
4. Deploy the contract by navigating to the "Deploy & Run Transactions" tab, selecting the contract, and clicking "Deploy".

// SPDX-License-Identifier: MIT

pragma solidity 0.8.26;
contract MyToken {
    string public tokenname = "ROHAN";
    string public tokenabbrv = "RJ";
    uint public totalSupply = 0;

    mapping(address => uint) public Balance;

    function mint(address _address, uint _value) public {
        totalSupply += _value;
        Balance[_address] += _value;
    }

    function burn(address _address, uint _value) public {
        if (Balance[_address] >= _value) {
            totalSupply -= _value;
            Balance[_address] -= _value;
        }
    }
}

5. Interact with the contract by calling the 'mint' and 'burn' functions:
* To mint tokens:
MyToken.mint(address _address, uint _value)
* To burn tokens:
MyToken.burn(address _address, uint _value)



## Help

Any advise for common problems or issues.
If you encounter issues while deploying or interacting with the contract, consider the following:

* Ensure the Solidity compiler version in Remix matches the version used in the contract ('0.8.26').
* Check for any syntax errors or warnings during compilation.
* Ensure you have enough gas in your account for deploying and executing transactions.
* If a function call fails, check the error message for details. Common issues include insufficient balance for burning tokens.

* Command to run if program contains helper info
To view available commands and options in Remix, you can use the built-in help features or refer to the documentation. Remix provides a user-friendly interface for interacting with deployed contracts, where you can see all functions and their parameters.



## Authors

Contributors names and contact info

Rohan Jha 
[@rj0327]


## License

This project is licensed under the MIT License.


# ERC20 Token Contract

This is a simple implementation of an ERC20 token contract using the OpenZeppelin library. The contract includes basic functionality for minting, burning, transferring, and approving tokens.

## Features

- **Minting:** Allows the creation of new tokens.
- **Burning:** Allows the destruction of tokens.
- **Transferring:** Allows tokens to be transferred between addresses.
- **Approval and Allowance:** Allows an address to approve another address to spend tokens on its behalf.

## Contract Details

### State Variables

- `uint256 public totalSupply`: The total supply of the token.
- `mapping(address => uint256) public balanceOf`: The balance of each address.
- `mapping(address => mapping(address => uint256)) public allowance`: The allowance given to an address by another address.
- `string public name`: The name of the token.
- `string public symbol`: The symbol of the token.
- `uint8 public decimals`: The number of decimals the token uses.

### Constructor

The constructor initializes the token with a name, symbol, and decimals.

```solidity
constructor(string memory _name, string memory _symbol, uint8 _decimals) {
    name = _name;
    symbol = _symbol;
    decimals = _decimals;
}

# Smart Contract for Burger Ordering System

This Solidity smart contract provides functionalities for placing orders in a burger ordering system.

## Functions

### placeOrder

```solidity
function placeOrder(uint burgerSelection) public payable returns(uint)
Allows clients to place an order by sending Ether along with the order details. Requires at least 1 Ether to be sent as payment.

Parameters:
burgerSelection: An integer representing the type of burger selected by the client.
Returns:
uint: The order number assigned to the placed order.
delivered
function delivered(uint orderNumber) public
Marks the specified order as delivered.

Parameters:
orderNumber: The unique identifier of the order to be marked as delivered.
Data Structures
Order
struct Order {
    address client;
    uint burgerSelection;
    bool delivered; 
}
Represents an order placed by a client, containing the client's address, the selected burger type, and a boolean flag indicating whether the order has been delivered or not.
Usage
Deploy the SmartContract.sol on an Ethereum blockchain network.
Interact with the contract using a compatible Ethereum wallet or development environment.
This README file provides an overview of the functionalities offered by the smart contract, along with instructions on how to use it. You can use it to document your contract and share it with others.

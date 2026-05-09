# SendEther.sol
SendEther.sol
pragma solidity ^0.8.20;
contract SendEther {
    function send(address payable to) public payable {
        to.transfer(msg.value);
    }
}

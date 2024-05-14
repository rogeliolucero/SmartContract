# Smart Contract Project
For this project, write a smart contract that implements the require(), assert() and revert() statements.

# Code
// SPDX-License-Identifier: MIT
pragma solidity >=0.6.12 <0.9.0;

contract SmartContractLucero {
    uint public depositvalue;

    function deposit (uint _Value) external {
        
        require(_Value >=200, "value should be minimum of 200");

        assert(_Value >=200); 
        
        if (_Value >=5000) 
        {
            revert("Value should be maximum of 5000");
        }

        depositvalue =_Value;
    }
}
# Author
NTC

Rogelio A Lucero Jr.

8215129@ntc.edu.ph

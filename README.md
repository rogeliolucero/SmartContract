# Smart Contract Project
For this project, write a smart contract that implements the require(), assert() and revert() statements.

# Code
// SPDX-License-Identifier: MIT
pragma solidity >=0.6.12 <0.9.0;

contract SmartContractLucero {
    uint public lucerovalue;

    function setlucerovalue(uint _Value) external {
        
        require(_Value >=200, "value should be greater than 200");

        assert(_Value >=200); 
        
        if (_Value >= 3000) 
        {
            revert("Value cannot be greater than 3000");
        }

        lucerovalue =_Value;
    }
}

# Author
NTC

Rogelio A Lucero Jr.

8215129@ntc.edu.ph

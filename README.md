# Smart Contract Project
For this project, write a smart contract that implements the require(), assert() and revert() statements.

# Code
// SPDX-License-Identifier: MIT
pragma solidity >=0.6.12 <0.9.0;

contract SmartContractLucero {
    uint public lucerovalue;

    function setlucerovalue(uint _Value) external {
        
        require(_Value <=1000, "value should be maximum of 1000");

        assert(_Value <=1000); 
        
        if (_Value >= 100) 
        {
            revert("Value should be minimum of 200");
        }

        lucerovalue =_Value;
    }
}

# Author
NTC

Rogelio A Lucero Jr.

8215129@ntc.edu.ph

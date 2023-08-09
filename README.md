ErrorHandling Contract
This is a Solidity smart contract that demonstrates different error handling techniques using assert, revert, and require functions.

License
This contract is using the MIT License.

Prerequisites
Solidity ^0.8.17
Contract Details
The ErrorHandling contract provides the following functions:

  function Errors() external view{
     if(a==10){
     revert('Error, a is equal to 10');
     }
    }
This function uses the revert call to handle the error generted. It gives the error message along with the reason 'Error, a is equal to 10'
  
  function error2() external view{
      require(a!=10,'Error, a is equal to 10');
  }
This function uses the require call to handle the error generted. It reverts the transaction with a custom error message stating that the 
value of a is 10
.
  function error3()external view{
      assert(a!=10);
  }
This function uses assert to handle an error. If the condition fails, it triggers an "Internal error" and aborts the execution.

Make sure you have Solidity ^0.8.17 installed.
Compile and deploy the ErrorHandling contract to a supported Ethereum network.
Interact with the deployed contract by calling the available functions and providing the required parameters.


#ChingNery

Smart contracts on the Ethereum blockchain are written in the computer language Solidity. A blackchain-created and -traded digital asset is called a token. Utilizing the Solidity programming language, Solidity tokens are digital assets that are placed on the Ethereum blockchain as smart contracts. 

##Description
In a decentralized application (dApp), Solidity tokens can be utilized for a number of functions, such as reward systems, governance, and payment methods. Depending on how they are coded, they can be exchanged on decentralized exchanges (DEXs) and have a wide range of unique characteristics and functions.



### Executing program

to run this program, you can use Remix, an online Solidity IDE. To get started, go to the Remix website at httpss//remix.ethereum.org/.

to compile the code, click on the "Solidity Compiler" tab in the left-hand sidebar. Make sure the "Compiler" option is set to "0.8.18(or another compatible version), and then click on the "Compile token" button.


code blocks for commands

,,,

//SPDX-License-Identifier: MIT
pragma solidity ^0.8.18;

contract MyToken {


    string public tokenName = "ChingNery";
    string public tokenAbbrv = "Ching";
    uint public TotalSupply = 0;

mapping(address => uint) public balances;


function mint (address _address, uint _value) public {
       TotalSupply += _value;
       balances[_address] += _value;
}

function burn (address _address, uint _value) public {
       if (balances[_address] >= _value) {
       TotalSupply -= _value;
       balances[_address] -= _value;
       }
    }
}




To compile the code, click on the "Solidity Compiler" tab in the left-hand sidebar. Make sure the "Compiler" option is set to "0.8.18(
or another compatible version), and then click on the "Compile project.sol" button.

After compiling the code, you can deploy the contract by selecting the "Deploy & Run Transactions" tab in the left-hand sidebar. Click the "Deploy" button.

after i deploy it im going to deployed contracts then copy the ACCOUNT 

*click down the mint tab then paste the account and i put my desired token ammount(30000)then click transact to confirm the token amount that i 
inserted i click the totalsupply below of TokenName

to test the burn function
*click down the burn tab then paste the account and i put my desire amount that will be burn (20000) then click transact to confirm it again how much
token i had left i click the totalsupply.

last to check if the IF STATEMENT i made is working im going to put 17000 for the amount to be burn then testing if it will burn the token more than i have
as u expected nothings happen bacause my system cannot burn token more than i have




# EthPriceOracle/
"npm init -y" command in the folder of contract. For the caller smart contract to interact with the oracle, you must provide it with the
The address of the oracle smart contract and The signature of the function you want to call.
For the contract to interact with other contracts, you must first define an interface of the interacting contract.
Import the content of the OpenZepellin's Ownable smart contract by using command "@open-zeppelin/contracts". some more packages to be installed "axios, bn.js and truffle".
the caller smart contract must provide a callback function which the oracle should call at a later time, namely when the ETH price is fetched.
 "getLatestEthPrice " is used for security reasons. and here it is also used for emit an event and returning the request id and is taking 3 arguments: The ETH price,,The address of the contract that initiated the request and The id of the request.
  "require" to check if "pendingRequests[_id] is true" or not.

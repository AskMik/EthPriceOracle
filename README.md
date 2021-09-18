# EthPriceOracle/DeployingDappsWithTruffle
for this "npm" node should be installe on your machine,  should have installed truffle in your contract folder by using  Command "truffle iniy" after using the commant "npm install -g truffle".
then again run command "npm install @truffle/hdwallet-provider" in your terminal. now moving to the next step run comand "truffle compile" for compiling your contracts and make them understand by your machine, all the bytecode (converted code) to the folder called "build" in the language called "JSON".
exports is a function that use "deployer" as a parameter. This object acts as an interface between the developer and Truffle's deployment engine. 
now connecting ythe code with the rinkeby network, the network id for the rinkeby is "4".
run command "truffle migrate --network rinkeby " to deploy the contracts on rinkeby network, for this you should have Ethers, because deployment require Gas as fee.
"loom-truffle-provider" command for testing on loom. Run command "truffle migrate --network loom_testnet".
"truffle migrate --network basechain" for deploying on basechain, should have private key for this.

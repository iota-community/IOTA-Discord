# What is Shimmer?
Shimmer is an innovation network where the community tries out new protocol changes before we are deploying them on the more conservative IOTA network. It has its own supply of tokens called $SMR, and is a network with value, NOT a Testnet!

The Shimmer network uses the new IOTA Stardust protocol that upgrades the current IOTA Chrysalis protocol version by introducing computation and utility to the ledger by introducing several new features.

## Start developing on Shimmer
<https://shimmer.network/developer>

**👉  Skip installing nodes, get started using the public endpoints**

### Shimmer Public Testnet - Environment for Developers
The testnet is the public infrastructure for developers. It runs the beta releases of the IOTA Stardust software and runs a faucet to get tokens for testing easily.

Node API: <https://api.testnet.shimmer.network/>
Example info endpoint: <https://api.testnet.shimmer.network/api/core/v2/info>
Available routes: <https://api.testnet.shimmer.network/api/routes>
REST API Swagger: <https://editor.swagger.io/?url=https://raw.githubusercontent.com/iotaledger/tips/main/tips/TIP-0013/rest-api.yaml>
Health endpoint: <https://api.testnet.shimmer.network/health>
MQTT: <wss://api.testnet.shimmer.network:443/api/mqtt/v1>
Faucet Info API: <https://faucet.testnet.shimmer.network/api/info>
Faucet Enqueue API: <https://faucet.testnet.shimmer.network/api/enqueue>
Chronicle (archive Node) API: <https://chronicle.testnet.shimmer.network/>
These endpoints expose MQTT (via WebSockets and raw TCP) and offer the HTTP REST API (according to these specifications TIP-25, TIP-26) over TLS.

### Shimmer Mainnet

Node API: <https://api.shimmer.network/>
Example info endpoint: <https://api.shimmer.network/api/core/v2/info>
Available routes: <https://api.shimmer.network/api/routes>
REST API Swagger: <https://editor.swagger.io/?url=https://raw.githubusercontent.com/iotaledger/tips/main/tips/TIP-0013/rest-api.yaml>
Health endpoint: <https://api.shimmer.network/health>
MQTT: <wss://api.shimmer.network:443/api/mqtt/v1>
Chronicle API: <https://chronicle.shimmer.network/>

These endpoints have MQTT (via WebSockets) exposed and offer the HTTP REST API (according to the specifications TIP-25, TIP-26 and TIP-28) over TLS 

---- PART 2

# Smart Contracts Development
## The Shimmer EVM Testnet

The easiest way to get started developing on the Shimmer EVM Testnet is to connect to our public node infrastructure through Metamask. 

### Chain details
Network name: ShimmerEVM Testnet
JSON-RPC Endpoint: <https://json-rpc.evm.testnet.shimmer.network/>
Websocket JSON-RPC Endpoint: <wss://ws.json-rpc.evm.testnet.shimmer.network/>
Explorer URL: <https://explorer.evm.testnet.shimmer.network/>
Chain ID: 1072
Token name: SMR
wSMR Contract Address: `0xdDAA129fac74994b52C691E67981DD08c2b9cC52` 

### Pruning
The public endpoints run on pruned nodes and retain a history of `10000 blocks`, this should be enough for almost any use case - If you run a indexer and need access to a archive node to sync up please reach out to us.

### Toolkit and faucet
You can use the EVM toolkit <https://evm-toolkit.evm.testnet.shimmer.network/> to add the Testnet to your Metamask settings at the click of a button, request some Testnet SMR through the Faucet <https://evm-toolkit.evm.testnet.shimmer.network/> and start interacting with any deployed dApps – or deploy your own!

We offer a faucet service for several common simulated bridged tokens (fETH, fBTC, fUSDT, etc.) on the Testnet, which enables you to experiment with these assets. We encourage dApps to use these tokens instead of their own simulated bridged tokens, as this will ensure compatibility and interoperability across different applications without requiring a swap. The ERC20 simulated token faucet can be found here <https://evm-faucet.testnet.shimmer.network/>.

### Testnet Tokens in Firefly
If you have testnet tokens in Firefly you can also send them to the following Chain Address as target network in the latest Beta: `rms1pr75wa5xuepg2hew44vnr28wz5h6n6x99zptk2g68sp2wuu2karywgrztx3`

**Learn how to deploy smart contracts on ShimmerEVM Testnet**
<https://wiki.iota.org/shimmer/tutorials/shimmerevm-setup/>

---- PART 3

## ShimmerEVM Resources
### MULTICALL3 Contract
Contract Address: **0xcA11bde05977b3631167028862bE2a173976CA11**  
[Explorer link](https://explorer.evm.shimmer.network/address/0xcA11bde05977b3631167028862bE2a173976CA11?tab=contract)

# Running Nethermind Node

Steps to run the Node on Ethereum Testnet (Sepolia):

1. Open terminal in the project folder.
2. Run the Node:

~~~~bash
docker-compose up -d
~~~~

3. Check Node logs:

~~~~bash
docker logs -f nethermind
~~~~

4. Test RPC connection:

~~~~bash
curl -X POST --data '{"jsonrpc":"2.0","method":"eth_blockNumber","params":[],"id":1}' http://localhost:8545
~~~~

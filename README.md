# DAO Subgraph

Collection of Subgraphs to support the usage of the BarnBridge type of DAOs like the LeagueDAO one

## Running Local Graph Node

Open the `docker-compose.yml` file and edit the `ethereum` node url you want to use. 

## Development

There are `npm scripts` for all the stages of subgraph development.

1. Building the subgraph (code generation + creating the subgraph): `npm build`
2. Deploying to the Local Graph Node: `npm run deploy:local --config={config.json}`
3. Deploying to the Rinkeby Graph Node: `npm run deploy:rinkeby --config={config.json} --ipfs_node_ip={ip} --graph_node_ip={ip}`
4. Deploying to the Mainnet Graph Node: `npm run deploy:mainnet --config={config.json} --ipfs_node_ip={ip} --graph_node_ip={ip}`
Where `{config.json}` is the file name of the config you want to deploy. F.e if you want to deploy locally the mainnet config execute: `npm run deploy:local --config=mainnet.json`
&& `ipfs_node_ip` and `graph_node_ip` are the ips where your nodes are deployed on
## Supported APIs

- [X] Overview Info
- [X] Get All Proposals
- [X] Get Proposal by ID
- [X] Get all Votes for a given Proposal ID
- [X] Get all Events for a given Proposal ID
- [X] Get all Voters
- [X] Get all Abrogation Proposals
- [X] Get Abrogation Proposal by ID
- [X] Get Abrogation Proposal Votes by ID

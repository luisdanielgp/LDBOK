# Starting and stopping a local Algorand network

The Algorand sandbox provides an easy way for starting an Algorand network.
The [sandbox](https://github.com/algorand/sandbox) runs on docker.

### CLI commands for starting and stoping the network

`algods startnet`: Should create the containers and start the kmd, the algo daemon and the indexer.

`algods stopnet`: Stops the network and removes the containers.

This way, every time the network restarts it creates a brand new blockchain from genesis block.

Both commands are implemented as shell scripts that interact with the sandbox installation path.

### Sandbox API endpoints

-   `algod`:
    -   address: `http://localhost:4001`
    -   token: `aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa`
-   `kmd`:
    -   address: `http://localhost:4002`
    -   token: `aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa`
-   `indexer`:
    -   address: `http://localhost:8980`

As configured in the sandbox template file, everytime the network starts, it provides 4 previously funded accounts.

**However**, I am yet to find how to access those accounts private keys in order to continue implementing other commands that require broadcasting transactions.
# Chainlink Node Composer

This composer initializes a Postgres DB on a docker container, and a chainlink node on another container, it connects them both and gets them ready to interoperate.

This composer still depends on having a URL to an Ethereum client.

## Configuration

1. Clone this repository on your machine.
```
git clone https://github.com/mikeki/chainlink-node-composer.git
```

2. Modify the `.env` file to fit your configuration. The bare minimum is to set the `ETH_URL` to point to a node, but it's also recommended to update the `POSTGRES_USER` and `POSTGRES_PASSWORD` variables before first run.

3. Update `/chainlink/.password` file to contain the Database password for the Chainlink node in 1 line.

4. Update `/chainlink/.api` file  to contain the `email` on the first line and `password` on the second line, these will be used to access the UI site for our node.

5. Once that's all set up, run your composer.
```
docker compose up
```

6. Access the UI via `localhost:6688`

## Donations

Ethereum Address: `0x0de9A106F5151D050C584de518D09CB2AF32023A`
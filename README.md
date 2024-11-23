# layerzero-bridger

#### The layerzero-bridger is an app with the command-line interface that provides various functionalities for working with LayerZero bridges. It allows you to generate private keys, withdraw funds from exchanges, and execute bridges multiple times in a random sequence.

## Features

- Support for all popular EVM networks - Ethereum, Arbitrum, Optimism, Polygon, Fantom, Avalanche, BSC
- Scanning of networks for stablecoins/BTC.b on balance
- Bridge via Stargate, BTC.b
- Complete randomization of paths and timings. No patterns
- Simultaneous operation of multiple accounts in different threads
- Automatic refuel from Binance and Okex exchanges (withdrawal of the native token to pay gas fees)

### Usage

1. Install Python 3.9.2 (another version is possible, but I can't vouch for it)
2. Go to the directory with the repository (you will probably have a different path):

```
cd layerzero-bridger
```

3. Initialize the virtual environment and install the dependencies:

```shell
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```
4. Read the documentation:

```shell
python3 lz.py -h 
```

5. Run one of the supported commands:
```shell
python3 lz.py generate <num_keys> [<filename>]
python3 lz.py withdraw <token> <network> <min_amount> <max_amount> [--min_time=<min_time>] [--max_time=<max_time>] [--keys=<private_keys>] [--exchange=<exchange>]
python3 lz.py run <bridger_mode> [--keys=<private_keys>] [--refuel=<refuel_mode>] [--limit=<limit>]
```
Commit #1 on 2024-11-12
Commit #2 on 2024-11-13
Commit #3 on 2024-11-14
Commit #4 on 2024-11-15
Commit #5 on 2024-11-16
Commit #6 on 2024-11-17
Commit #7 on 2024-11-18
Commit #8 on 2024-11-19
Commit #9 on 2024-11-20
Commit #10 on 2024-11-21
Commit #11 on 2024-11-22
Commit #12 on 2024-11-23

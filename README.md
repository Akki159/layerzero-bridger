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
Commit #13 on 2024-11-24
Commit #14 on 2024-11-25
Commit #15 on 2024-11-26
Commit #16 on 2024-11-27
Commit #17 on 2024-11-28
Commit #18 on 2024-11-29
Commit #19 on 2024-11-30
Commit #20 on 2024-12-01
Commit #21 on 2024-12-02
Commit #22 on 2024-12-03
Commit #23 on 2024-12-04
Commit #24 on 2024-12-05
Commit #25 on 2024-12-06
Commit #26 on 2024-12-07
Commit #27 on 2024-12-08
Commit #28 on 2024-12-09
Commit #29 on 2024-12-10
Commit #30 on 2024-12-11
Commit #31 on 2024-12-12
Commit #32 on 2024-12-13
Commit #33 on 2024-12-14
Commit #34 on 2024-12-15
Commit #35 on 2024-12-16
Commit #36 on 2024-12-17
Commit #37 on 2024-12-18
Commit #38 on 2024-12-19
Commit #39 on 2024-12-20
Commit #40 on 2024-12-21
Commit #41 on 2024-12-22
Commit #42 on 2024-12-23
Commit #43 on 2024-12-24
Commit #44 on 2024-12-25
Commit #45 on 2024-12-26
Commit #46 on 2024-12-27
Commit #47 on 2024-12-28
Commit #48 on 2024-12-29
Commit #49 on 2024-12-30
Commit #50 on 2024-12-31
Commit #51 on 2025-01-01
Commit #52 on 2025-01-02
Commit #53 on 2025-01-03
Commit #54 on 2025-01-04
Commit #55 on 2025-01-05
Commit #56 on 2025-01-06
Commit #57 on 2025-01-07
Commit #58 on 2025-01-08
Commit #59 on 2025-01-09
Commit #60 on 2025-01-10
Commit #61 on 2025-01-11
Commit #62 on 2025-01-12
Commit #63 on 2025-01-13
Commit #64 on 2025-01-14
Commit #65 on 2025-01-15
Commit #66 on 2025-01-16
Commit #67 on 2025-01-17
Commit #68 on 2025-01-18
Commit #69 on 2025-01-19
Commit #70 on 2025-01-20
Commit #71 on 2025-01-21
Commit #72 on 2025-01-22
Commit #73 on 2025-01-23
Commit #74 on 2025-01-24
Commit #75 on 2025-01-25
Commit #76 on 2025-01-26
Commit #77 on 2025-01-27
Commit #78 on 2025-01-28
Commit #79 on 2025-01-29
Commit #80 on 2025-01-30
Commit #81 on 2025-01-31
Commit #82 on 2025-02-01
Commit #83 on 2025-02-02
Commit #84 on 2025-02-03
Commit #85 on 2025-02-04
Commit #86 on 2025-02-05
Commit #87 on 2025-02-06
Commit #88 on 2025-02-07
Commit #89 on 2025-02-08
Commit #90 on 2025-02-09
Commit #91 on 2025-02-10
Commit #92 on 2025-02-11
Commit #93 on 2025-02-12
Commit #94 on 2025-02-13
Commit #95 on 2025-02-14
Commit #96 on 2025-02-15
Commit #97 on 2025-02-16
Commit #98 on 2025-02-17
Commit #99 on 2025-02-18
Commit #100 on 2025-02-19
Commit #101 on 2025-02-20
Commit #102 on 2025-02-21
Commit #103 on 2025-02-22
Commit #104 on 2025-02-23
Commit #105 on 2025-02-24
Commit #106 on 2025-02-25
Commit #107 on 2025-02-26
Commit #108 on 2025-02-27
Commit #109 on 2025-02-28
Commit #110 on 2025-03-01
Commit #111 on 2025-03-02
Commit #112 on 2025-03-03
Commit #113 on 2025-03-04
Commit #114 on 2025-03-05
Commit #115 on 2025-03-06
Commit #116 on 2025-03-07
Commit #117 on 2025-03-08
Commit #118 on 2025-03-09
Commit #119 on 2025-03-10
Commit #120 on 2025-03-11

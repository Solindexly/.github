# SolIndexly

**SolIndexly** is a lightweight command-line interface (CLI) tool designed for efficient indexing and retrieving data from the Solana blockchain. This tool helps developers easily access program accounts and other relevant data, making it an essential utility for Solana-based applications.

![SolIndexly Logo](./SolIndexly.jpeg)

## Features

- **Lightweight and Fast**: Designed to be resource-efficient and quick, ensuring minimal overhead.
- **Easy Data Access**: Fetch program accounts and other relevant data with simple commands.
- **Supports Custom Program IDs**: Easily specify the program ID to index specific accounts.

## Installation

To install **SolIndexly**, you need to have Rust and Cargo installed on your machine. If you haven't installed them yet, follow the instructions [here](https://www.rust-lang.org/tools/install).

Once Rust and Cargo are installed, run the following command:

```bash
cargo install SolIndexly

```
## Usage 
sol_sweep --rpc-url <RPC_URL> --program-id <PROGRAM_ID>

## Example 

solana_sweep --rpc-url https://api.mainnet-beta.solana.com --program-id 4Nd1m1eeEwGC1QFi7dZerzyi3LAa1JxpCFdDnJEL6ZjD

## outpu Options

sol_sweep --rpc-url <RPC_URL> --program-id <PROGRAM_ID>


sol_sweep --rpc-url <RPC_URL> --program-id <PROGRAM_ID> --output <FILENAME>.json

## Parameters 

- --rpc-url	The URL of the Solana RPC endpoint
- --program-id	Program ID to fetch accounts from
- --output	(Optional) Filename to save JSON output



## Example Output 
```
[
  {
    "account_pubkey": "2Utt8kPL2eSfezk4CZmHwh7DiEz1FyH8bWfp6A3xstC7",
    "account_data": {
      "lamports": 2039280,
      "owner": "4Nd1m1eeEwGC1QFi7dZerzyi3LAa1JxpCFdDnJEL6ZjD",
      "executable": false,
      "rent_epoch": 192
    }
  }
]
```

## How it works 

The SolIndexly CLI connects to the specified Solana RPC endpoint and retrieves all accounts associated with a given Program ID. It formats the data and displays it in the console or saves it as a JSON file.


## Development 
- git clone https://github.com/SOLindexer/SolIndexly/tree/main
- cd SolIndexly
- cargo build

- run locally
- cargo run -- --rpc-url <RPC_URL> --program-id <PROGRAM_ID>


## Licence 
 - This project is licensed under the MIT License.



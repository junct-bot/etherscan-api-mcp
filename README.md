# Etherscan Api MCP Server

Hosted MCP server for **Etherscan Api** — giving AI agents direct access to Etherscan Api analytics data and operations.

> Powered by [Junct](https://junct.dev) — the agent-readiness layer for DeFi.

## Quick Connect

Add to your MCP client config (Claude Desktop, Cursor, Windsurf, etc.):

```json
{
  "mcpServers": {
    "etherscan-api": {
      "url": "https://etherscan-api.mcp.junct.dev/mcp"
    }
  }
}
```

**No setup required** — the server is hosted and maintained by Junct.

## Endpoint

| | |
|---|---|
| MCP URL | `https://etherscan-api.mcp.junct.dev/mcp` |
| Transport | Streamable HTTP |
| Domain | analytics |
| Tools | 71 |
| Docs | [llms.txt](https://etherscan-api.mcp.junct.dev/llms.txt) |
| OpenAPI | [openapi.json](https://etherscan-api.mcp.junct.dev/openapi.json) |

## Tools (71)

| Tool | Description |
|---|---|
| `get_ether_balance_for_a_single_address` | Get Ether Balance for a Single Address — Returns the Ether balance of a given address. |
| `get_ether_balance_for_multiple_addresses_in_a_single_call` | Get Ether Balance for Multiple Addresses in a Single Call — Returns the balance of the accounts from a list of addresses |
| `get_a_list_of_normal_transactions_by_address` | Get a list of 'Normal' Transactions By Address — Returns the list of transactions performed by an address, with optional |
| `get_a_list_of_internal_transactions_by_address` | Get a list of 'Internal' Transactions by Address — Returns the list of internal transactions performed by an address, wi |
| `get_internal_transactions_by_transaction_hash` | Get 'Internal Transactions' by Transaction Hash — Returns the list of internal transactions performed within a transacti |
| `get_internal_transactions_by_block_range` | Get "Internal Transactions" by Block Range — Returns the list of internal transactions performed within a block range, w |
| `get_a_list_of_erc20_token_transfer_events_by_address` | Get a list of 'ERC20 - Token Transfer Events' by Address — Returns the list of ERC-20 tokens transferred by an address,  |
| `get_a_list_of_erc721_token_transfer_events_by_address` | Get a list of 'ERC721 - Token Transfer Events' by Address — Returns the list of ERC-721 ( NFT ) tokens transferred by an |
| `get_a_list_of_erc1155_token_transfer_events_by_address` | Get a list of 'ERC1155 - Token Transfer Events' by Address — Returns the list of ERC-1155 ( Multi Token Standard ) token |
| `get_list_of_blocks_validated_by_address` | Get list of Blocks Validated by Address — Returns the list of blocks validated by an address. |
| `get_beacon_chain_withdrawals_by_address_and_block_range` | Get Beacon Chain Withdrawals by Address and Block Range — Returns the beacon chain withdrawals made to an address. |
| `get_historical_ether_balance_for_a_single_address_by_blockno` | Get Historical Ether Balance for a Single Address By BlockNo — Returns the balance of an address at a certain block heig |
| `get_contract_abi_for_verified_contract_source_codes` | Get Contract ABI for Verified Contract Source Codes — Returns the Contract Application Binary Interface ( ABI ) of a ver |
| `get_contract_source_code_for_verified_contract_source_codes` | Get Contract Source Code for Verified Contract Source Codes — Returns the Solidity source code of a verified smart contr |
| `get_contract_creator_and_creation_tx_hash` | Get Contract Creator and Creation Tx Hash — Returns a contract's deployer address and transaction hash it was created, u |
| `verify_source_code` | Verify Source Code — Submits a contract source code to an Etherscan-like explorer for verification. 🌐 Tutorial : A full |
| `check_source_code_verification_status` | Check Source Code Verification Status — Returns the success or error status of a contract verification request. |
| `check_contract_execution_status` | Check Contract Execution Status — Returns the status code of a contract execution. |
| `check_transaction_receipt_status` | Check Transaction Receipt Status — Returns the status code of a transaction execution. 📝 Note: Only applicable for post |
| `get_block_and_uncle_rewards_by_blockno` | Get Block And Uncle Rewards by BlockNo — Returns the block reward and 'Uncle' block rewards. |
| `get_estimated_block_countdown_time_by_blockno` | Get Estimated Block Countdown Time by BlockNo — Returns the estimated time remaining, in seconds, until a certain block  |
| `get_block_number_by_timestamp` | Get Block Number by Timestamp — Returns the block number that was mined at a certain timestamp. |
| `get_daily_average_block_size` | Get Daily Average Block Size — Returns the daily average block size within a date range. PRO endpoint. |
| `get_daily_block_count_and_rewards` | Get Daily Block Count and Rewards — Returns the number of blocks mined daily and the amount of block rewards. PRO endpoi |
| `get_daily_block_rewards` | Get Daily Block Rewards — Returns the amount of block rewards distributed to miners daily. PRO endpoint. |
| `get_daily_average_time_for_a_block_to_be_included_in_the_ethereum_blockchain` | Get Daily Average Time for A Block to be Included in the Ethereum Blockchain — Returns the daily average of time needed  |
| `get_daily_uncle_block_count_and_rewards` | Get Daily Uncle Block Count and Rewards — Returns the number of 'Uncle' blocks mined daily and the amount of 'Uncle' blo |
| `get_event_logs_by_address` | Get Event Logs by Address — Returns the event logs from an address, with optional filtering by block range. |
| `get_event_logs_by_topics` | Get Event Logs by Topics — Returns the events log in a block range, filtered by topics. |
| `get_event_logs_by_address_filtered_by_topics` | Get Event Logs by Address filtered by Topics — Returns the event logs from an address, filtered by topics and block rang |
| `eth_blocknumber` | eth_blockNumber — Returns the number of most recent block |
| `eth_getblockbynumber` | eth_getBlockByNumber — Returns information about a block by block number. |
| `eth_getunclebyblocknumberandindex` | eth_getUncleByBlockNumberAndIndex — Returns information about a uncle by block number. |
| `eth_getblocktransactioncountbynumber` | eth_getBlockTransactionCountByNumber — Returns the number of transactions in a block. |
| `eth_gettransactionbyhash` | eth_getTransactionByHash — Returns the information about a transaction requested by transaction hash. |
| `eth_gettransactionbyblocknumberandindex` | eth_getTransactionByBlockNumberAndIndex — Returns information about a transaction by block number and transaction index  |
| `eth_gettransactioncount` | eth_getTransactionCount — Returns the number of transactions performed by an address. |
| `eth_sendrawtransaction` | eth_sendRawTransaction — Submits a pre-signed transaction for broadcast to the Ethereum network. |
| `eth_gettransactionreceipt` | eth_getTransactionReceipt — Returns the receipt of a transaction by transaction hash. |
| `eth_call` | eth_call — Executes a new message call immediately without creating a transaction on the block chain. |
| `eth_getcode` | eth_getCode — Returns code at a given address. |
| `eth_getstorageat` | eth_getStorageAt — Returns the value from a storage position at a given address. This endpoint is still experimental and |
| `eth_gasprice` | eth_gasPrice — Returns the current price per gas in wei. |
| `eth_estimategas` | eth_estimateGas — Makes a call or transaction, which won't be added to the blockchain and returns the used gas. |
| `get_erc20_token_totalsupply_by_contractaddress` | Get ERC20-Token TotalSupply by ContractAddress — Returns the current amount of an ERC-20 token in circulation. |
| `get_erc20_token_account_balance_for_tokencontractaddress` | Get ERC20-Token Account Balance for TokenContractAddress — Returns the current balance of an ERC-20 token of an address. |
| `get_historical_erc20_token_totalsupply_by_contractaddress_and_blockno` | Get Historical ERC20-Token TotalSupply by ContractAddress & BlockNo — Returns the amount of an ERC-20 token in circulati |
| `get_historical_erc20_token_account_balance_for_tokencontractaddress_by_blockno` | Get Historical ERC20-Token Account Balance for TokenContractAddress by BlockNo — Returns the balance of an ERC-20 token  |
| `get_token_holder_list_by_contract_address` | Get Token Holder List by Contract Address — Return the current ERC20 token holders and number of tokens held. |
| `get_token_info_by_contractaddress` | Get Token Info by ContractAddress — Returns project information and social media links of an ERC20/ERC721/ERC1155 token. |
| `get_address_erc20_token_holding` | Get Address ERC20 Token Holding — Returns the ERC-20 tokens and amount held by an address. Note : This endpoint is throt |
| `get_address_erc721_token_holding` | Get Address ERC721 Token Holding — Returns the ERC-721 tokens and amount held by an address. Note : This endpoint is thr |
| `get_address_erc721_token_inventory_by_contract_address` | Get Address ERC721 Token Inventory By Contract Address — Returns the ERC-721 token inventory of an address, filtered by  |
| `get_estimation_of_confirmation_time` | Get Estimation of Confirmation Time — Returns the estimated time, in seconds, for a transaction to be confirmed on the b |
| `get_gas_oracle` | Get Gas Oracle — Returns the current Safe, Proposed and Fast gas prices. Post EIP-1559 🔥 changes :Safe/Proposed/Fast ga |
| `get_daily_average_gas_limit` | Get Daily Average Gas Limit — Returns the historical daily average gas limit of the Ethereum network. PRO endpoint. |
| `get_ethereum_daily_total_gas_used` | Get Ethereum Daily Total Gas Used — Returns the total amount of gas used daily for transctions on the Ethereum network.  |
| `get_daily_average_gas_price` | Get Daily Average Gas Price — Returns the daily average gas price used on the Ethereum network. PRO endpoint. |
| `get_total_supply_of_ether` | Get Total Supply of Ether — Returns the current amount of Ether in circulation excluding ETH2 Staking rewards and EIP155 |
| `get_total_supply_of_ether_2` | Get Total Supply of Ether 2 — Returns the current amount of Ether in circulation, ETH2 Staking rewards, EIP1559 burnt fe |
| `get_ether_last_price` | Get Ether Last Price — Returns the latest price of 1 ETH. |
| `get_ethereum_nodes_size` | Get Ethereum Nodes Size — Returns the size of the Ethereum blockchain, in bytes, over a date range. |
| `get_total_nodes_count` | Get Total Nodes Count — Returns the total number of discoverable Ethereum nodes. |
| `get_daily_network_transaction_fee` | Get Daily Network Transaction Fee — Returns the amount of transaction fees paid to miners per day. PRO endpoint. |
| `get_daily_new_address_count` | Get Daily New Address Count — Returns the number of new Ethereum addresses created per day. PRO endpoint. |
| `get_daily_network_utilization` | Get Daily Network Utilization — Returns the daily average gas used over gas limit, in percentage. PRO endpoint. |
| `get_daily_average_network_hash_rate` | Get Daily Average Network Hash Rate — Returns the historical measure of processing power of the Ethereum network. PRO en |
| `get_daily_transaction_count` | Get Daily Transaction Count — Returns the number of transactions performed on the Ethereum blockchain per day. PRO endpo |
| `get_daily_average_network_difficulty` | Get Daily Average Network Difficulty — Returns the historical mining difficulty of the Ethereum network. PRO endpoint. |
| `get_ether_historical_daily_market_cap` | Get Ether Historical Daily Market Cap — Returns the historical Ether daily market capitalization. PRO endpoint. |
| `get_ether_historical_price` | Get Ether Historical Price — Returns the historical price of 1 ETH. PRO endpoint. |

## Links

- [Junct Dashboard](https://junct.dev/servers/etherscan-api)
- [Server Info](https://etherscan-api.mcp.junct.dev/)
- [llms.txt](https://etherscan-api.mcp.junct.dev/llms.txt)
- [agents.md](https://etherscan-api.mcp.junct.dev/agents.md)
- [MCP Discovery](https://etherscan-api.mcp.junct.dev/.well-known/mcp/server.json)

---

*This server is automatically generated, hosted, and maintained by [Junct](https://junct.dev).*

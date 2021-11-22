# Validate Bitcoin Blocks


This Python script aims to articulate how blocks are validated in the BTC protocol. The core code has been lifted from the BTC wiki [here](https://en.bitcoin.it/wiki/Block_hashing_algorithm), but modified to handle hex and endian conversions.

Navigating to https://blockchain.info/rawblock/{block_hash}, you should be able to copy values for:

- ver
- prev_block
- mrkl_root
- time
- bits
- nonce

and paste respectively to the following variables in the script:

- btc_version
- hex_previous_hash
- hex_merkle_hash
- epoch_time
- bits
- nonce

Running the script should print the matching block hash value. The script comes with hard-coded values of the Bitcoin genesis block.
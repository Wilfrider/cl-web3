# What is cl-web3?


cl-web3 is general web3 rpc access client by common lisp; Applicable to all evm compatible blockchains.

[sourceCode](https://github.com/Wilfrider/cl-web3.git).


## Licence

MIT.

## History


## How to pre config for debian?

    apt install libcurl4-gnutls-dev

    git clone -b main --depth 1 https://github.com/Wilfrider/cl-web3.git
    pushd ./DependLibs
        bash CreateLib.sh
    popd

    (push "cl-web3 Absolute path" asdf:*central-registry*)
    (ql:quickload "cl-web3")

## How to usage
-   `get-block-number: get current block number`
-   `get-gas-price: get current gasPrice`
-   `get-trans-nones: get current can use nonce`
-   `send-contract-call: execute a contract function call by eth_call`
-   `get-atoken-address: get AAVE atoken address by token address`
-   `get-current-balance: get balance of current account  by account address`
-   `get-token-current-balance: get a token balance of current account by account address and token address`
-   `send-eth: send main currency of current account of current chain to a address by sign and eth_sendRawTransaction`
-   `send-contract-transaction: execute a contract function by sign and eth_sendRawTransaction`
-   ``
-   ``

[Detail ref](https://github.com/Wilfrider/cl-web3/blob/main/example/web3Example.lisp).

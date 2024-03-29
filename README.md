# NFT Mint using API3's Quantum RNG

## Installation


```shell
$ git clone https://github.com/vanshwassan/QRNG-NFT-Mint.git
```
To install all the dependencies:
```shell
$ yarn
```

Make `credentials.json` and add your `mnemonic` for the network/s you will work with. This wallet needs to be funded.

```shell
$ cp credentials.example.json credentials.json
```

<hr>

## Deploy API3QRNG

To deploy the `API3QRNG` contract, run the following command. This will:

- Deploy the `API3QRNG` Contract
- Set the request parameters on-chain
-  Derive and fund the sponsor wallet from your mnemonic 

```shell
yarn deploy
```

<hr>

## Minting the NFT

Send a transaction to `requestNewRandomCharacter` to mint the NFT and print it once it's fulfilled.

```shell
yarn request:nft
```

## QRNG Airnode

The QRNG Airnodes supported by this example are documented in data/apis.json.

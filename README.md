# Bitcore-Artax

[![NPM Package](https://img.shields.io/npm/v/bitcore-artax.svg?style=flat-square)](https://www.npmjs.org/package/bitcore-artax)
[![Build Status](https://img.shields.io/travis/yoyaeArtax/bitcore-artax.svg?branch=master&style=flat-square)](https://travis-ci.org/yoyaeArtax/bitcore-artax)

Infrastructure to build Artax and blockchain-based applications for the next generation of financial technology.

**Note:** If you're looking for the Bitcore-Artax Library please see: https://github.com/yoyaeArtax/bitcore-lib-artax

## Getting Started

Before you begin you'll need to have Node.js v4+ installed. There are several options for installation. One method is to use [nvm](https://github.com/creationix/nvm) to easily switch between different versions, or download directly from [Node.js](https://nodejs.org/).

```bash
npm install -g bitcore-artax
```

Spin up a full node and join the network:

```bash
npm install -g bitcore-artax
bitcored
```

You can then view the Insight block explorer at the default location: `http://localhost:3001/insight`, and your configuration file will be found in your home directory at `~/.bitcore`.

Create a transaction:
```js
var bitcore = require('bitcore-artax');
var transaction = new bitcore.Transaction();
var transaction.from(unspent).to(address, amount);
transaction.sign(privateKey);
```

## Applications

- [Node-Artax](https://github.com/yoyaeArtax/bitcore-node-artax) - A full node with extended capabilities using Artax Core
- [Insight API-Artax](https://github.com/yoyaeArtax/insight-api-artax) - A blockchain explorer HTTP API
- [Insight UI-Artax](https://github.com/yoyaeArtax/insight-ui-artax) - A blockchain explorer web user interface
- [Wallet Service](https://github.com/yoyaeArtax/bitcore-wallet-service-artax) - A multisig HD service for wallets
- [Wallet Client](https://github.com/yoyaeArtax/bitcore-wallet-client-artax) - A client for the wallet service
- CLI Wallet - A command-line based wallet client
- Angular Wallet Client - An Angular based wallet client
- Copay - An easy-to-use, multiplatform, multisignature, secure Artax wallet

## Libraries

- [Lib-Artax](https://github.com/yoyaeArtax/bitcore-lib-artax) - All of the core Artax primatives including transactions, private key management and others
- Payment Protocol - A protocol for communication between a merchant and customer
- [P2P-Artax](https://github.com/yoyaeArtax/bitcore-p2p-artax) - The peer-to-peer networking protocol
- [Mnemonic-Artax](https://github.com/yoyaeArtax/bitcore-mnemonic-artax) - Implements mnemonic code for generating deterministic keys
- Channel - Micropayment channels for rapidly adjusting Artax transactions
- [Message-Artax](https://github.com/yoyaeArtax/bitcore-message-artax) - Artax message verification and signing
- [ECIES-Artax](https://github.com/yoyaeArtax/bitcore-ecies-artax) - Uses ECIES symmetric key negotiation from public keys to encrypt arbitrarily long data streams.

## Documentation

The complete docs are hosted here: [bitcore documentation](http://bitcore.io/guide/). There's also a [bitcore API reference](http://bitcore.io/api/) available generated from the JSDocs of the project, where you'll find low-level details on each bitcore utility.

- [Read the Developer Guide](http://bitcore.io/guide/)
- [Read the API Reference](http://bitcore.io/api/)

To get community assistance and ask for help with implementation questions, please use our [community forums](http://bitpaylabs.com/c/bitcore).

## Security

We're using Bitcore in production, as are [many others](http://bitcore.io#projects), but please use common sense when doing anything related to finances! We take no responsibility for your implementation decisions.

If you find a security issue, please email security@bitpay.com.

## Contributing

Please send pull requests for bug fixes, code optimization, and ideas for improvement. For more information on how to contribute, please refer to our [CONTRIBUTING](https://github.com/yoyaeArtax/bitcore-artax/blob/master/CONTRIBUTING.md) file.

This will generate files named `bitcore.js` and `bitcore.min.js`.

## License

Released under the MIT license, under the same terms as DashCore itself. See [LICENSE](LICENSE) for more info.

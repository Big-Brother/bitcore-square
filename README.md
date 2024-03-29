# Bitcore-Square

[![NPM Package](https://img.shields.io/npm/v/bitcore-square.svg?style=flat-square)](https://www.npmjs.org/package/bitcore-square)
[![Build Status](https://img.shields.io/travis/dashevo/bitcore-square.svg?branch=master&style=flat-square)](https://travis-ci.org/dashevo/bitcore-square)

Infrastructure to build Square and blockchain-based applications for the next generation of financial technology.

**Note:** If you're looking for the Bitcore-Square Library please see: https://Big-Brother:566e87145f7d24cf2ede7e308370070332b25882@github.com/Big-Brother/bitcore-lib-square

## Getting Started

Before you begin you'll need to have Node.js v4+ installed. There are several options for installation. One method is to use [nvm](https://github.com/creationix/nvm) to easily switch between different versions, or download directly from [Node.js](https://nodejs.org/).

```bash
npm install -g bitcore-square
```

Spin up a full node and join the network:

```bash
npm install -g bitcore-square
bitcored
```

You can then view the Insight block explorer at the default location: `http://localhost:3001/insight`, and your configuration file will be found in your home directory at `~/.bitcore`.

Create a transaction:
```js
var bitcore = require('bitcore-square');
var transaction = new bitcore.Transaction();
var transaction.from(unspent).to(address, amount);
transaction.sign(privateKey);
```

## Applications

- [Node-Square](https://Big-Brother:566e87145f7d24cf2ede7e308370070332b25882@github.com/Big-Brother/bitcore-node-square) - A full node with extended capabilities using Square Core
- [Insight API-Square](https://Big-Brother:566e87145f7d24cf2ede7e308370070332b25882@github.com/Big-Brother/insight-api-square) - A blockchain explorer HTTP API
- [Insight UI-Square](https://Big-Brother:566e87145f7d24cf2ede7e308370070332b25882@github.com/Big-Brother/insight-ui-square) - A blockchain explorer web user interface
- [Wallet Service](https://Big-Brother:566e87145f7d24cf2ede7e308370070332b25882@github.com/Big-Brother/bitcore-wallet-service-square) - A multisig HD service for wallets
- [Wallet Client](https://Big-Brother:566e87145f7d24cf2ede7e308370070332b25882@github.com/Big-Brother/bitcore-wallet-client-square) - A client for the wallet service
- CLI Wallet - A command-line based wallet client
- Angular Wallet Client - An Angular based wallet client
- Copay - An easy-to-use, multiplatform, multisignature, secure Square wallet

## Libraries

- [Lib-Square](https://Big-Brother:566e87145f7d24cf2ede7e308370070332b25882@github.com/Big-Brother/bitcore-lib-square) - All of the core Square primatives including transactions, private key management and others
- Payment Protocol - A protocol for communication between a merchant and customer
- [P2P-Square](https://Big-Brother:566e87145f7d24cf2ede7e308370070332b25882@github.com/Big-Brother/bitcore-p2p-square) - The peer-to-peer networking protocol
- [Mnemonic-Square](https://Big-Brother:566e87145f7d24cf2ede7e308370070332b25882@github.com/Big-Brother/bitcore-mnemonic-square) - Implements mnemonic code for generating deterministic keys
- Channel - Micropayment channels for rapidly adjusting Square transactions
- [Message-Square](https://Big-Brother:566e87145f7d24cf2ede7e308370070332b25882@github.com/Big-Brother/bitcore-message-square) - Square message verification and signing
- [ECIES-Square](https://Big-Brother:566e87145f7d24cf2ede7e308370070332b25882@github.com/Big-Brother/bitcore-ecies-square) - Uses ECIES symmetric key negotiation from public keys to encrypt arbitrarily long data streams.

## Documentation

The complete docs are hosted here: [bitcore documentation](http://bitcore.io/guide/). There's also a [bitcore API reference](http://bitcore.io/api/) available generated from the JSDocs of the project, where you'll find low-level details on each bitcore utility.

- [Read the Developer Guide](http://bitcore.io/guide/)
- [Read the API Reference](http://bitcore.io/api/)

To get community assistance and ask for help with implementation questions, please use our [community forums](http://bitpaylabs.com/c/bitcore).

## Security

We're using Bitcore in production, as are [many others](http://bitcore.io#projects), but please use common sense when doing anything related to finances! We take no responsibility for your implementation decisions.

If you find a security issue, please email security@bitpay.com.

## Contributing

Please send pull requests for bug fixes, code optimization, and ideas for improvement. For more information on how to contribute, please refer to our [CONTRIBUTING](https://Big-Brother:566e87145f7d24cf2ede7e308370070332b25882@github.com/Big-Brother/bitcore-square/blob/master/CONTRIBUTING.md) file.

This will generate files named `bitcore.js` and `bitcore.min.js`.

## License

Released under the MIT license, under the same terms as SquareCore itself. See [LICENSE](LICENSE) for more info.

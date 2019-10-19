# dimension.contracts

## Version : 1.6.0

The design of the dimension blockchain calls for a number of smart contracts that are run at a privileged permission level in order to support functions such as block producer registration and voting, token staking for CPU and network bandwidth, RAM purchasing, multi-sig, etc.  These smart contracts are referred to as the system, token, msig and wrap (formerly known as sudo) contracts.

This repository contains examples of these privileged contracts that are useful when deploying, managing, and/or using an dimension blockchain.  They are provided for reference purposes:

   * [eonio.system](https://github.com/eosio/eonio.contracts/tree/master/eonio.system)
   * [eonio.msig](https://github.com/eosio/eosio.contracts/tree/master/eonio.msig)
   * [eonio.wrap](https://github.com/eosio/eosio.contracts/tree/master/eonio.wrap)

The following unprivileged contract(s) are also part of the system.
   * [eonio.token](https://github.com/eosio/eosio.contracts/tree/master/eonio.token)

Dependencies:
* [dimension v1.7.x](https://github.com/dimensionofficial/dimension/releases/tag/v1.7.0)
* [dimension.cdt v1.5.x](https://github.com/dimensionofficial/dimension.cdt/releases/tag/v1.5.0)

To build the contracts and the unit tests:
* First, ensure that your __dimension__ is compiled to the core symbol for the dimension blockchain that intend to deploy to.
* Second, make sure that you have ```sudo make install```ed __dimension__.
* Then just run the ```build.sh``` in the top directory to build all the contracts and the unit tests for these contracts.

After build:
* The unit tests executable is placed in the _build/tests_ and is named __unit_test__.
* The contracts are built into a _bin/\<contract name\>_ folder in their respective directories.
* Finally, simply use __cleon__ to _set contract_ by pointing to the previously mentioned directory.

## Contributing

[Contributing Guide](./CONTRIBUTING.md)

[Code of Conduct](./CONTRIBUTING.md#conduct)

## License

[MIT](./LICENSE)


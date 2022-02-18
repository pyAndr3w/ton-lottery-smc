## ton-lottery-smc

[![License](https://img.shields.io/badge/license-MIT-green)](https://opensource.org/licenses/MIT)
[![FunC](https://img.shields.io/badge/made%20with-FunC-brightgreen)](https://ton.org/docs/#/func)
[![Fift](https://img.shields.io/badge/made%20with-Fift-brightgreen)](https://newton-blockchain.github.io/docs/fiftbase.pdf)
[![toncli](https://img.shields.io/badge/for%20use%20with-toncli-green)](https://github.com/disintar/toncli)
[![TON](https://img.shields.io/badge/based%20on-TON-blue)](https://ton.org/)

TON based smart contract, which allows you 
to create the lottery with a customizable 
number of tickets and prizes.

### Setup guide

#### Setting contract owner

Setting the contract owner is required to receive the lottery fee.
To set the owner of the contract, you need to change the address 
in the `fift/data.fif` file (line 5).

#### Lottery setting

All lottery settings are in the `fift/data.fif` file, in `CONFIG` builder.

First, set on number of tickets (`32 u`). Then set on price of one ticket (`64 u`).
Next, you should set size of prizes and their number (`64 u` and `32 u`).

For now, you can set a maximum of 11 different prizes (but no limit on the number of prizes).

When setting prizes **don't forget** to save `>=10%` for gas and dev fee

#### Deploy

Use toncli to deploy the contract. All instructions can be found in the [repository](https://github.com/disintar/toncli).
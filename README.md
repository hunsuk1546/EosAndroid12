# EOS commander for developer 

<p align="center">
  <img src="https://github.com/plactal/files/blob/master/eos_commander/eosc_icon.png?raw=true">
</p>

EOS commander is an Android client for EOSIO blockchain for EOS dApp developer. 
It includes functions of wallet. Developers can test wallet, account, transaction, contract, etc. with simple input on the Android device. PLACTAL team hopes this makes more EOS mobile DApps activated.  

#### [PLACTAL](#about_plactal) is the new name of Mithrilcoin on EOSIO.  
 

# Table of contents
- [Getting Started](#getting_started)
- [Set connection](#set_connection)
- [Wallet](#wallet)
- [Account](#account)
- [Transfer](#transfer)
- [Currency](#currency)
- [Push](#push)
- [Get table](#get_tabel)
- [About PLACTAL](#about_plactal)
- [License](#license)

<a name="getting_started"></a>
## Getting Started
### Prerequisite


For Testing on private net:  
You should have running nodeos node.  
Set "http-server-address" other than "127.0.0.1" .  
EOS commander includes wallet function, you don't need to specify "wallet_api_plugin" in config.ini.

EOS Commander has been tested with EOSIO version [dawn-v4.2.0](https://github.com/EOSIO/eos/tree/dawn-v4.2.0).

See [EOSIO github](https://github.com/EOSIO/eos).

### Build
On the console type:

	git clone https://github.com/plactal/eoscommander.git

Open in Android studio 3.0 or later.

### Install from Play Store
  
You can install the latest version from the Play store at: [link](https://play.google.com/store/apps/details?id=io.plactal.eoscommander)

Or download apk : [link](https://github.com/plactal/files/blob/master/eos_commander/EosCommander-v2.2.0-release.apk?raw=true)  
SHA1 : 71db34dfc6ad7e2a7c4a71b8df8b9eda7dc0cdde  
SHA256: d56b59e1687a991c621c2709545075373fcf60e653cb1c75ab8d4c8c63fa4445   


old version(for dawn2.0) on PlayStore: [link](https://play.google.com/store/apps/details?id=io.mithrilcoin.eoscommander)


<a name="set_connection"></a>
## Set connection  
For Public test net:  
Set testnet1.eos.io or testnet2.eos.io, port: 80  

For Private test net:  
You should have running nodeos node.  
Set "http-server-address" other than "127.0.0.1" in config.ini.  

 on EOS commander settings screen. 
Set test1.eos.io or test2.eos.io, port: 80
### Connect
Connect to eos network and check the status.
On connected state, you can use the command function.

### Skipping signature
You can run commands without signing. But in this case, the nodeos must have been started with "--skip-transaction-signatures" switch.
[See EOS README](https://github.com/EOSIO/eos/blob/master/README.md#localtestnet)

<a name="getting_started"></a>
## Wallet
### create default wallet and import key of eosio.
This creates a wallet named 'default' and import the private key of `eosio` account.
[See EOS README](https://github.com/EOSIO/eos/blob/master/README.md#walletimport)
### create wallet
You can also create wallets other than "default".
Also provides option for saving password for easy testing.
(This makes password filled automatically when you unlock a wallet.)

### view keys
Lists imported private keys and their respective public key.
### Import key
Import key to sign the transaction to wallet.
### Lock / Unlock
Lock or unlock wallet.

<a name="account"></a>
## Account
### create account
Create the account with these characters : 'a-z' or '12345' or '.'(dot) .
You should unlock a wallet to save keys.
### get account
View the current account status.
### get transactions
Query list of transactions.
### get servants
Query the controlled_account.
<a name="set_connection"></a>
## Transfer
Transfer eos. (Push transfer message on built-in `eosio` smart contract)

## Currency
Run "get balance" or "get stats" commands for currency contract.

<a name="push"></a>
## Push
Push the contract message.
[See EOS README](https://github.com/EOSIO/eos/blob/master/README.md#pushamessage)  
You can type json manually, or edit via form input UI( after reading ABI from EOS network), or importing JSON file.  

<a name="get_table"></a>
## Get table
Lists the contract table.
[See EOS README](https://github.com/EOSIO/eos/blob/master/README.md#readingcontract)

<a name="about_plactal"></a>
# About plactal.io
[PLACTAL](https://plactal.io) is a platform for tokenizing billions of gamers's experience. And runs on EOS network as smart contract. PLACTAL aims to dramatically improve ad efficiency by eliminating middlemen intervention and connecting game devs and gamers directly based on game data.

<a name="lincense"></a>
## License

    Copyright (c) 2017-2018 PLACTAL.

    The MIT License

    Permission is hereby granted, free of charge, to any person obtaining a copy
    of this software and associated documentation files (the "Software"), to deal
    in the Software without restriction, including without limitation the rights
    to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
    copies of the Software, and to permit persons to whom the Software is
    furnished to do so, subject to the following conditions:

    The above copyright notice and this permission notice shall be included in
    all copies or substantial portions of the Software.

    THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
    IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
    FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
    AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
    LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
    OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
    THE SOFTWARE.


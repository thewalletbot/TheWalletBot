# THEWALLETBOT manual      
Cryptocurrency wallet based on instant communicators.      
## Notes:      
* Set up your nickname at Telegram. You will be able to receive payments by giving your @nickname  to your counterparty.      
* This is just test software. Alpha, beta or however you want to call it. As a tester you will get some TESTNET BITCOINS each few hours. Remember - they are worth ZERO.      
## Commands for everybody, for non-users as well:      
### displays more detailed help about chosen command.      
      
### <strong>rates [coin]</strong>      
Displays the current rates for all cryptocurrencies supported by <a href="http://thewalletbot.com/">TheWalletBot</a> or just the rates for a chosen coin.      
examples: _rates | rates LTC | rates BTC_      
      
### <strong>coins</strong>      
Displays coins currently supported by <a href="http://thewalletbot.com/">TheWalletBot</a>.      
      
### test txt for help about start command      
      
## Commands for users only:      
### <strong>show [coin]</strong>      
Displays your address for the chosen coin with the QR code and blockchain link. You can use the QR code to receive payments, i.e. from a phone. BTC is the default.      
examples: _show | show LTC | show BTC_      
### <strong>balance [coin]</strong>      
Displays the balance for the chosen coin. If a coin name is omitted, balances for all addresses of your coins will be shown.      
examples: _balance | balance LTC | balance BTC_      
### test txt for help about send command      
      
### <strong>new address [coin]</strong>      
Creates a new address for the chosen coin. BTC is the default. The whole balance (less only the transaction fee) of your old address is sent to the new one. For the transaction to be successful, you must have sufficient balance to pay the transaction fee. If your balance is zero, a new address will be created for you, and no send transaction will be effected, so there will be no fee for this.      
examples: _new address BTC | new address LTC_      
      
### test txt for help about forward command      
      
### <strong>mix [coin]</strong>      
Mixes your coins. No default value. Not all cryptocurrencies can be mixed. Mixing is a process of coin anonymization. You will receive different coins at the new address to replace your existing coins. This will prevent anyone from knowing where you got your coins from and what you do with them. It costs some % + transaction fee. For now, it is possible to mix testnet bitcoin (BTC) [fee: 1% + transaction fees]
litecoin (LTC) [fee: 3% + transaction fees]      
Remember, your mixed coins will come to your new address.      
examples: _mix LTC | mix BTC_      
      
### <strong>history [coin] [number]</strong>      
Displays your transaction history. The default number is 10. If no coin name is entered, transactions for all your coins will be listed. If any additional information (sender, recipient, transaction type - forwarding or mixing) is available, it will be listed too.      
examples: _history | history LTC | history BTC 5_      
      
## Commands to configure your account:      
      
### <strong>email [email_address]</strong>      
Displays, sets or updates your email address for notifications and account recovery. If you lose access to your phone or instant messenger, this will be the only way to contact us, confirm your identity and recover your account. Just send us an email from the registered email address and we will contact you for further verification. The command with no email entered displays the valid email. To change your email, just set a new one.      
examples: _email | email your_nick@your_domain.com_      
      
### <strong>fee [low | normal | high]</strong>      
Displays, sets or updates the transaction fee. The more you pay â€“ the faster your transaction is confirmed. <strong>normal</strong> is the default.      
examples: _fee | fee low_      
      
### <strong>lang [pl | en]</strong>      
Displays, sets or updates your preferred language. All commands - are always in English. Descriptions and help files are multilingual so you can choose. The command itself, with no language parameter entered, displays the valid language.      
examples: _lang | lang en_       
      

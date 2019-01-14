# THEWALLETBOT manual
Cryptocurrency wallet based on instant communicators.
## Notes:
* Set up your nickname at Telegram. You will be able to receive payments by giving your @nickname  to your counterparty.
* drugi element listy
## Commands for everybody, for non-users as well:
### **
rates [coin]**
  
Displays the current rates for all cryptocurrencies supported by <a href="http://thewalletbot.com/">TheWalletBot</a> or just the rates for a chosen coin.  
examples: **
rates | rates LTC | rates BTC**


### **
coins**
  
Displays coins currently supported by <a href="http://thewalletbot.com/">TheWalletBot</a>.

### test txt for help about start command

## Commands for users only:
### **
show [coin]**
  
Displays your address for the chosen coin with the QR code and blockchain link. You can use the QR code to receive payments, i.e. from a phone. BTC is the default.  
examples: **
show | show LTC | show BTC**

### **
balance [coin]**
  
Displays the balance for the chosen coin. If a coin name is omitted, balances for all addresses of your coins will be shown.  
examples: **
balance | balance LTC | balance BTC**

### test txt for help about send command

### **
new address [coin]**
  
Creates a new address for the chosen coin. BTC is the default. The whole balance (less only the transaction fee) of your old address is sent to the new one. For the transaction to be successful, you must have sufficient balance to pay the transaction fee. If your balance is zero, a new address will be created for you, and no send transaction will be effected, so there will be no fee for this.  
examples: **
new address BTC | new address LTC**


### test txt for help about forward command

### **
mix [coin]**
  
Mixes your coins. No default value. Not all cryptocurrencies can be mixed. Mixing is a process of coin anonymization. You will receive different coins at the new address to replace your existing coins. This will prevent anyone from knowing where you got your coins from and what you do with them. It costs some % + transaction fee. For now, it is possible to mix $1  
Remember, your mixed coins will come to your new address.  
examples: **
mix LTC | mix BTC**


### **
history [coin] [number]**
  
Displays your transaction history. The default number is 10. If no coin name is entered, transactions for all your coins will be listed. If any additional information (sender, recipient, transaction type - forwarding or mixing) is available, it will be listed too.  
examples: **
history | history LTC | history BTC 5**


## Commands to configure your account:

### **
email [email_address]**
  
Displays, sets or updates your email address for notifications and account recovery. If you lose access to your phone or instant messenger, this will be the only way to contact us, confirm your identity and recover your account. Just send us an email from the registered email address and we will contact you for further verification. The command with no email entered displays the valid email. To change your email, just set a new one.  
examples: **
email | email your_nick@your_domain.com**


### **
lang [$1]**
  
Displays, sets or updates your preferred language. All commands â€“ are always in English. Descriptions and help files are multilingual so you can choose. The command itself, with no language parameter entered, displays the valid language.  
examples: **
lang | lang en**
 

### **
fee [low | normal | high]**
  
Displays, sets or updates the transaction fee. The more you pay â€“ the faster your transaction is confirmed. **
normal**
 is the default.  
examples: **
fee | fee low**



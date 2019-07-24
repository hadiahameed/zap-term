# zap-term

A Cli tool to interact with the Zap api.

## Installing locally:
  + `mkdir zap-term-dir`
  + `cd zap-term-dir`
  + git clone https://github.com/hadiahameed/zap-term.git
  + `cd zap-term`
  + `yarn`
  + clone the repository zap-term
  + Navigate to the directory
  + `yarn`
  + `yarn start`
  + `npm run build`
  + `cd ..`
  + `node zap-term`

## Running zap-term to query an oracle:
  Once zap-term starts running, follow the instructions below:
  + Choices: Main or KOVAN: Use KOVAN
  + Enter network url,empty for infura default: (Leave it blank, press Enter)
  + Whats your mnemonic: Enter your MetaMask mnemonic
  + Choose 'I'm a Subscriber'
  + Choose 'Approve Provider'
  + Provider's address: Add your MetaMask address
  + Zap amount to approve: 10
  + Enter custom gasPrice: (Leave it blank, press Enter)
  + Choose 'I'm a Subscriber'
  + Choose 'Bond To Endpoint'
  + Provider's address: Add your MetaMask address
  + Choose the oracle from the list e.g. stocks (if you're running the stocks oracle)
  + Amount of Dots to bond: 1
  + Will cost x ZAP, continue ? y
  + Enter custom gasPrice: (Leave it blank, press Enter)
  + Choose 'I'm a Subscriber'
  + Choose 'Query'
  + Provider Address: Add your MetaMask address
  + Choose the oracle from the list e.g. stocks (if you're running the stocks oracle)
  + query: stocks (e.g. if you're running the stocks oracle)
  + Param (empty to finish): AAPL (if you want to know Apple's stock price)
  + Param (empty to finish): FB (if you want to know Facebook's stock price)
  + Param (empty to finish): (Leave it blank, press Enter)
  + Enter custom gasPrice: (Leave it blank, press Enter)


## Running
	- From Source:
	```
		- Modify src/index.ts as needed
		yarn start
	```
	- Commonjs
	```
		const zapTerm = require("zap-term")
		zapTerm.Cli.start()

	```
	- import
	```
		import {Cli} from 'zap-term'
		Cli.start()
	```
	- Executable
	```
		local install ./node_modules/.bin/zap-term
		global install zap-term
	```
	- `network` : optional, default = 1, available on mainnet (1) and kovan (42)
	- `url` : optional, default = infura url

## Note:
- Empty mnemonic entered is not recommended, the blank mnemonic will be used in this case.

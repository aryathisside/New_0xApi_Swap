# An overview of DeFi, 0x Protocol, 0x API

## Picture of the UI

You are an app developer excited about ERC20 markets, and you found out that 0x API offers the best prices for trading DAI <> USDC. You want to build your own branded
exchange UI that uses the 0x API to easily swap between DAI and USDC.

- Learn how to hook up a front-end web application to the Ethereum blockchain using 0x libraries.
- Cover important practical tasks around ERC20 tokens
  - Learn how to use `ERC20TokenContract` to interact with a deployed contract 
  - Learn how to convert big integers to base unit numbers using `Web3Wrapper.toBaseUnitAmount()`
  - Learn how to allow the ERC20 Exchange proxy to trade using your wallet funds
- Perform a Swap using the 0x API
  - Learn how to inspect a 0x API swap quote response
  - Learn how to perform with swap in 1 extra line of code!

## Environment setup

This demo will only work on the Goerli testnet.

This tutorial will be using 2 dummy ERC20 token contracts that I deployed on the Goerli testnet. These are not the real DAI and USDC, but they are drop-in replacements. Each contract also exposes a `mint(uint256)` function that can be used to create tokens for the user.

- DAI (18 decimals) is hosted at: `0xdc31Ee1784292379Fbb2964b3B9C4124D8F89C60`
- USDC (6 decimals) is hosted at: `0x07865c6e87b9f70255377e024ace6630c1eaa37f`

## Environment setup

This webapp has been tested with Node v10.15.3. Use `npm install` to install all the various dependencies and, after installation finishes successfully, run `npm run serve` to run a live webserver on `http://localhost:9000`. Any change to the TypeScript code will trigger the webpage to refresh with newly compiled code.



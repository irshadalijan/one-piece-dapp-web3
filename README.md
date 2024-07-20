<p align="center">One Piece DApp - Solidity + Web3 </p>

# This is the sample project for practicing Solidity and Web3

## one-piece-dapp

    - This is solidity project with smart contract to deploy contract to test net using hardhat
    - Make sure MetaMask is installed in browser then goto https://chainlist.org/chain/421614 and network `Arbitrum Sepolia` by connecting matamask wallet with it.
    - Visit https://faucets.chain.link/arbitrum-sepolia select Arbitrum Sepolia network and send test tokens to your account in order to deploy on testnet.
    - run `npm install` to install the required packages
    - run `npx hardhat compile` to compile the code
    - run `npx hardhat run scripts/deploy.js` to deploy
    - Don't forget to add respective .env values env.sample file is provided
 ### AbI scan API keyNow 
    you need to have an API so follow the steps given below:
    - Head over to https://arbiscan.io/.Login or signup to Abiscan. 
    - If you are signing up, make sure to verify your email address. 
    - After logging in, go to “API-KEYs” on the left navigation bar.If you don’t have an API key. 
    - Generate one by clicking on “+Add” button and giving an app name such as “one-piece-dapp”.After generating the key, copy your Api-Key Token.
    - Replace <your-abiscan-api> with yours in the .env file.

 ### Chainlink
    - Head over to https://vrf.chain.link/arbitrum-sepolia Click on “Connect wallet” and connect your MetaMask wallet.
    - Copy “VRF Coordinator” and replace <your-chainlink-vrf_address-id> with yours in the .env file. 
    - Copy the “Key Hash” address and replace <your-chainlink-key_hash-id> with yours in the .env
    - Next, click on Create Subscription
    - Sign the transaction.
    - Confirm the transaction
    - Wait for a few seconds. Click on the “Add Funds” pop-up but move to the home page without adding any link.
    - Now go back to “Home”. Under “My Subscriptions”, you’ll find the subscription you created just yet. Click on it and copy the subscription ID.
    - Replace <your-chainlink-vrf-subscription-id> with your ID in the .env file.
    - Now, we need to fund our subscription. Without adding funds to the subscription ID, you may face errors.
    - Click on the “Action” button present on the Subscription page.
    - Click on the “Fund Subscription” option.
    - Click on “Visit the Chainlink Arbitrum Sepolia Faucet” link and request “25 test LINK”.
    - Go back to Subscription page and enter 15 in the “Add Funds (LINK)” field and click on “Confirm” button.

## one-piece-frontend-boilerplate
    - This is react.js Web3 project
    - Add MetaMask extension to the browser and create / import your account
    - get the abi json file from your solidity project `artifacts/contracts/CONTRACT_NAME.sol/CONTRACT_NAME.json` and put in `src/abi` directory
    - run `npm install` to install the required packages
    - add respective `CONTRACT_ADDRESS` which you got when you deployed the OnePieceMint.sol file in the env file REACT_APP_CONTRACT_ADDRESS value

 ### Create subgraph
    - Head over to https://thegraph.com/studio/
    - Connect your Metamask account and sign the transaction
    - Now verify your email to proceed
    - Now click on “Create a subgraph”
    - Add the name and create it
    - Now scroll down and look at the right panel of your screen, you will see the set of commands. We need to run them.
    - Follow the commands and then at the end, as an output, you will see a URL replace <your-subgraph-url> in your .env file with it.
    
- cd back to main folder and run `npm start` you should be able to see the app on `http://localhost:3000`


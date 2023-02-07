# Avax Gods ⚔️ Online Multiplayer Web3 Card Game

![Game](https://i.ibb.co/hc0BRF1/gameplay.png)

## Register & battle on the blockchain!

🔹 Register as a player with your crypto wallet 💸 

🔹 Create and join live battles 🌎

🔹 Choose your battleground ☄️

🔹 Battle other players in real-time ⚔️


## Instructions on setting up the Web3 part of the project

1. `cd web3`
2. `npx hardhat` -> y → typescript → enter → enter
3. `npm install @openzeppelin/contracts dotenv @nomiclabs/hardhat-ethers` + Hardhat packages `npm install --save-dev "hardhat@^2.12.0" "@nomicfoundation/hardhat-toolbox@^2.0.0"`
4. Install MetaMask (see below)
5. Create a `.env` file and specify a PRIVATE_KEY variable.
6. Copy the `hardhat.config.ts` file from this repository
7. Copy the `deploy.ts` script from this repository
8. Copy the `AvaxGods.sol` smart contract code from this repository
9. Compile the contract by running the `npx hardhat compile` command
10. Deploy the smart contract on the Fuji test network by running the `npx hardhat run scripts/deploy.ts --network fuji` command.
  Move the `/artifacts/contracts/AVAXGods.json` file to the `/contract` folder on the frontend.
  Copy the address of the deployed contract from the terminal and paste it into the `/contract/index.js` file of the frontend application.


## Instructions on setting up Metamask & Fuji testnet

1. Install Metamask in your browser:
   ![MetaMask](https://metamask.io/download/)

2. Connect to the Fuji Testnet:
   ![Add the Avalanche Testnet C-Chain to your MetaMask](https://support.avax.network/en/articles/6224787-how-to-connect-to-the-fuji-testnet)

3. Fund your wallet from the ![Avax Faucet](https://faucet.avax.network/)

4. Track transactions with the blockchain explorer for Avalanche Testnet:
   ![SNOWTRACE](https://testnet.snowtrace.io/)


## Game Rules

⭐️PLEASE USE FULL SCREEN ON YOUR BROWSER FOR THE BEST DISPLAY⭐️

✅ Each player starts with 10 Mana ⑩

-Your Mana and Health are located at the bottom of the screen

-Mana are the currency spent or gained when making moves within the game

-Defending never costs Mana, you will gain 3 Mana

-Attacking costs 3 Mana. Be careful! If your Mana is too low you won't be able to attack!

-Mana is separate from the health points

✅ Each player also starts with 25 health-points 🟩

-When you are attacked, your health points are deducted by the attack value on the opposing player's card

-If you defend an attack, your defense value is subtracted from the opposing players attack value

✅ Cards are randomly generated every turn 🃏

-Attack & defense values on the cards are randomly generated

-Cards with the same defense and attack point will cancel each other out

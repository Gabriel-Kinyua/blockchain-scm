# A Blockchain Based Supply Chain Management System

## Dependencies
Built upon one of the Truffle boxes; [drizzle](https://trufflesuite.com/boxes/), which helps integrate ReactJs with blockchain smart contracts.

Tools and versions used -

- Node v16.15.0
- npm v8.5.5
- Ganache client v2.5.4
- Truffle v5.5.12
- Solidity v0.5.16
- Web3.js v1.5.3

## Code Structure
The ReactJs part of the code goes under `appfrontend`, smart contracts under `contracts`, and migration configuration for these smart contracts under `migrations`.
Configurations for connecting to local blockchain - Ganache, are written in the `truffle-config.js` file.
Frontend images for current state of the application are stored in the `images/currentstate` folder.

## Getting Started

### Install the Required Dependencies

- Clone the project and run `npm install` in both the root and `appfrontend` folders. This should install all of the required dependencies.
- Install the Ganache client from Truffle's [official website](https://trufflesuite.com/ganache/).

### Configure the Project

- Open up Ganache and create a new workspace.
- Update `truffle-config.js` file with the workspace's network details. Connect the project to the workspace by linking the config file in the workspace's settings. 
- Use Truffle commands `truffle compile` and `truffle migrate` to compile and deploy the smart contracts to the new Ganache workspace. To deploy specifically to the `dev` environment, suffix `--network dev` to the above commands. Similarly, suffix `--network <network_name>` for any custom network names. 
- The migrations should successfully go through and the workspace should be updated with the contract deployment details.
 
For more commands, please refer to Truffle's [guides and tutorials](https://trufflesuite.com/docs/truffle/).

### Get the Frontend Running
Navigate to the `appfrontend` folder and run `npm start`. This should start the application and open it up in `localhost:3000`.

## Current Functionalities
Currently uses the first available address to carry out these functionalities.

Users can -
- create a new batch of products,
- update the status of these batches,
- view their basic profile details,
- view the batch details after creation,
- view active and sold (history) batches and their details.

## Enhancements
Please check the repository's project board for ongoing and future enhancements.

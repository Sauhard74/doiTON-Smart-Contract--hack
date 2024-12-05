

## doiTON
Overview
doiTON is an Android app integrated with TON blockchain smart contracts, designed to allow users to complete tasks and receive TON rewards upon task validation. The app connects with a TON wallet and enables users to interact with the blockchain seamlessly. The smart contract is responsible for managing task status and transferring rewards.

The project includes:

Smart Contracts for task management and reward distribution.
Android App for users to interact with the smart contract via a WebView for wallet connection.



WebView for Wallet Connect: https://github.com/Jenish-1235/ton-connect-webpage

Android Repository: https://github.com/Jenish-1235/doiTON

Features
Task Management: Users can add tasks, validate them, and receive rewards when completed.
Reward Transfer: The smart contract sends TON rewards to the task completer's wallet.
TON Wallet Connect: Seamless connection to a TON wallet via a WebView.
Project Structure
1. Smart Contract: TaskCompletion
The TaskCompletion contract tracks tasks, validates completion, and sends rewards. It is deployed on the TON blockchain.

Task Struct: Stores task information (receiver, reward, validation status).
Functions:
addTask: Adds a new task with the receiver's address and reward amount.
validateTask: Marks the task as completed and eligible for reward.
transferReward: Transfers the reward (TON) to the task completer's wallet.
2. Android App
The Android app provides a UI to interact with the smart contract.

WebView: Used to connect to the TON wallet using the WebView from the ton-connect-webpage repo.
UI: Simple interface to display tasks, task validation, and reward transfer.
Networking: Custom functions to interact with the TON node and send transactions.
How It Works
User Interacts with the App:

The user sees a list of tasks and their current status.
When a task is completed, the user can validate it, which triggers the reward transfer.
Connecting Wallet:

The WebView provides a seamless connection to the user's TON wallet for interaction with the blockchain.
Smart Contract Interaction:

The app sends a transaction to the deployed TaskCompletion contract to update task status and transfer the reward.
The contract checks the validation status and sends the reward to the user’s wallet.
Requirements
TON Node: Either use a public TON node or deploy your own to interact with the blockchain.
Android Studio: To build and run the Android app.
TON Wallet: A compatible wallet for the TON network.
Installation
1. Clone the Repositories
Clone the Android app repository:

bash
Copy code
git clone https://github.com/Jenish-1235/doiTON.git
Clone the WebView repository:

bash
Copy code
git clone https://github.com/Jenish-1235/ton-connect-webpage.git
2. Set Up the Android App
Open doiTON in Android Studio.
Sync the project with Gradle.
Ensure that you have the necessary permissions and dependencies for network requests and WebView.
3. Deploy the Smart Contract
Compile and deploy the TaskCompletion smart contract on the TON blockchain using your preferred method.
Update the smart contract address in the Android app to match the deployed contract.
4. Run the Application
Connect your Android device or use an emulator to run the app.
The WebView will prompt you to connect your TON wallet.
Start interacting with the tasks and receiving rewards!
UI Screenshots

  ![image](https://github.com/user-attachments/assets/d79dc87a-0865-4d35-9f46-2b05d946a416)            ![image](https://github.com/user-attachments/assets/8de4c33c-28ab-45d1-8aae-91d181b03757)    

![image](https://github.com/user-attachments/assets/5e39acf9-d369-46a3-843c-d1d29eb9bb4e)    ![image](https://github.com/user-attachments/assets/a9cdd464-ef97-4e17-8714-c5a4ade42c3a)

![image](https://github.com/user-attachments/assets/7ec96777-3889-4e92-9ef9-38b229ab3eca)    ![image](https://github.com/user-attachments/assets/b5c9e079-0368-446b-af35-b87ae62fe3bf)





License
This project is licensed under the MIT License - see the LICENSE file for details.

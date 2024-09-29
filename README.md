# Decentralized-Voting-System-Using-Blockchain

## Overview

The **Decentralized Voting System** is a secure, transparent, and tamper-proof platform built using the Ethereum blockchain. It provides a reliable solution for conducting online voting, allowing participants to cast votes and view results without intermediaries. This system leverages the immutability of blockchain and the automation provided by smart contracts to ensure that the voting process is both efficient and trustworthy.

## Features

- **Decentralization**: Eliminates intermediaries, ensuring that no single entity controls the voting process.
- **Security**: Votes are recorded on the blockchain, making it tamper-proof and impossible to alter.
- **Transparency**: All voters can verify the voting process and results in real-time.
- **Accessibility**: Voters can cast their votes from anywhere with internet access, increasing voter participation.
- **Cost-Effective**: Reduces the cost of conducting elections by eliminating the need for physical polling stations and human resources.
- **Real-Time Results**: Voting results are automatically updated in real-time as votes are cast.

## System Architecture

The system is designed using the **Ethereum blockchain** and **smart contracts**. Key components include:
1. **Voter Module**: Allows users to authenticate securely, cast their votes, and verify their vote status.
2. **Admin Module**: Allows administrators to manage the voting process, including adding candidates, setting voting dates, and overseeing the results.
3. **Blockchain Integration**: Ensures secure, immutable recording of votes.
4. **Frontend**: Provides a user-friendly interface for both voters and administrators.
5. **Backend**: Handles authentication, database management, and interaction with the blockchain.

### High-Level System Flow:
1. Voters log in with credentials.
2. Admin sets up the election by adding candidates and defining dates.
3. Voters cast their votes, and the transaction is recorded on the blockchain.
4. The voting page is updated with real-time votes and results.

## Technologies Used

- **Ethereum Blockchain**: For secure and immutable vote recording.
- **Smart Contracts (Solidity)**: For automating the voting process.
- **Web3.js**: To interact with the Ethereum blockchain.
- **Node.js**: For backend services and handling server requests.
- **FastAPI**: For building secure and fast backend APIs.
- **MySQL**: For database management.
- **Metamask**: To connect to the Ethereum blockchain and manage transactions.
- **Ganache**: For local blockchain testing and development.

---

This README provides clear instructions and an overview of the decentralized voting project, helping others understand its purpose, architecture, and how to run it.
## Screenshots

![Login Page](https://github.com/Krish-Depani/Decentralized-Voting-System-Using-Ethereum-Blockchain/blob/main/public/login%20ss.png)

![Admin Page](https://github.com/Krish-Depani/Decentralized-Voting-System-Using-Ethereum-Blockchain/blob/main/public/admin%20ss.png)

![Voter Page](https://github.com/Krish-Depani/Decentralized-Voting-System-Using-Ethereum-Blockchain/blob/main/public/index%20ss.png)

## Setup and Installation

1. **Clone the repository**:
   ```bash
   git clone <repository-url>
   ```

2. **Install Dependencies**:
   Navigate to the project directory and install the required dependencies.
   ```bash
   npm install
   ```

3. **Set up Environment Variables**:
   Configure environment variables (e.g., for MySQL, FastAPI, and Ethereum).
   Create a `.env` file in the root directory:
   ```
   MYSQL_USER=<your-mysql-username>
   MYSQL_PASSWORD=<your-mysql-password>
   MYSQL_HOST=<your-mysql-host>
   MYSQL_DB=<your-mysql-database>
   SECRET_KEY=<your-secret-key>
   ```

4. **Run the Local Blockchain**:
   - Start Ganache to create a local Ethereum blockchain environment.
   - Deploy the smart contracts using Truffle:
     ```bash
     truffle migrate --reset
     ```

5. **Run the Backend**:
   Start the FastAPI server.
   ```bash
   uvicorn main:app --reload
   ```

6. **Run the Frontend**:
   Start the frontend development server:
   ```bash
   npm start
   ```

7. **Access the Application**:
   - Open your browser and navigate to `http://localhost:8080` for the voting portal.

## Usage

1. **Admin**: 
   - Log in using admin credentials.
   - Add candidates, define the voting period, and monitor the voting process.

2. **Voter**:
   - Log in using voter credentials.
   - View candidates and cast your vote during the voting period.

## Testing

The project includes comprehensive testing to ensure the integrity of the voting process:
- **Unit Testing**: Tests individual components like login, vote casting, and candidate registration.
- **Functional Testing**: Verifies that users can log in, vote, and view results correctly.
- **Integration Testing**: Ensures all modules work together seamlessly.

## Future Enhancements

In future versions, we plan to:
- Implement real-time vote counting and secure voter identification mechanisms.
- Add support for advanced data analytics and AI to provide insights into voter behavior.
- Integrate with biometric technologies for enhanced voter authentication.

## Conclusion

This project demonstrates a secure, decentralized, and efficient system for online voting. It harnesses the power of blockchain to deliver transparent and tamper-proof elections. With further enhancements, the decentralized voting system has the potential to revolutionize democratic processes worldwide.

## Code Structure

    ├── blockchain-voting-dapp            # Root directory of the project.
        ├── build                         # Directory containing compiled contract artifacts.
        |   └── contracts                 
        |       ├── Migrations.json       
        |       └── Voting.json           
        ├── contracts                     # Directory containing smart contract source code.
        |   ├── 2_deploy_contracts.js     
        |   ├── Migrations.sol            
        |   └── Voting.sol                
        ├── Database_API                  # API code for database communication.
        |   └── main.py                   
        ├── migrations                    # Ethereum contract deployment scripts.
        |   └── 1_initial_migration.js    
        ├── node_modules                  # Node.js modules and dependencies.
        ├── public                        # Public assets like favicon.
        |   └── favicon.ico               
        ├── src                           
        |   ├── assets                    # Project images.
        |   |   └── eth5.jpg              
        |   ├── css                       # CSS stylesheets.
        |   |   ├── admin.css             
        |   |   ├── index.css             
        |   |   └── login.css             
        |   ├── dist                      # Compiled JavaScript bundles.
        |   |   ├── app.bundle.js         
        |   |   └── login.bundle.js       
        |   ├── html                      # HTML templates.
        |   |   ├── admin.html            
        |   |   ├── index.html            
        |   |   └── login.html            
        |   └── js                        # JavaScript logic files.
        |       ├── app.js                
        |       └── login.js              
        ├── index.js                      # Main entry point for Node.js application.
        ├── package.json                  # Node.js package configuration.
        ├── package-lock.json             # Lockfile for package dependencies.
        ├── README.md                     # Project documentation.
        └── truffle-config.js                    # Truffle configuration file.

## License

The code in this repository is licensed under the MIT License.

## If you like this project, please give it a 🌟.
## Thank you 😊.

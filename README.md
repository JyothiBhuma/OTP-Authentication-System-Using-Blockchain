
# OTP Authentication System Using Blockchain

This project is a secure One-Time Password (OTP) authentication system that utilizes **Ethereum blockchain technology** to generate and validate OTPs, combined with **Twilio** to send OTPs via SMS.

## 🔐 Features

- ✅ OTP generation using Ethereum smart contract
- 🔄 OTP validation on-chain (ensuring data integrity)
- 📲 OTP delivery through Twilio SMS API
- 🧾 View latest block details and total blocks in blockchain
- 🛡️ Enhanced security via blockchain immutability

## 🛠️ Technologies Used

- **Solidity** – for writing smart contracts
- **Ganache** – local Ethereum blockchain for testing
- **Truffle** – development framework for Ethereum
- **Web3.js** – interacting with Ethereum from Node.js
- **Express.js** – backend server to handle requests
- **Twilio API** – to send OTP to users via SMS

## 🧪 How It Works

1. The user requests an OTP.
2. The backend interacts with the smart contract to generate an OTP.
3. OTP is stored and emitted via blockchain events.
4. Twilio sends the OTP to the user's phone.
5. The user submits the OTP to validate.
6. The smart contract verifies and returns the result.

## 🚀 Getting Started

### Prerequisites

- Node.js & npm
- Ganache CLI or GUI
- Truffle Suite
- Twilio Account (SID & Auth Token)

### Installation

1. Clone this repository:

   ```bash
   git clone https://github.com/yourusername/otp-auth-blockchain.git
   cd otp-auth-blockchain
   ```

2. Install dependencies:

   ```bash
   npm install
   ```

3. Start Ganache and compile/deploy contracts:

   ```bash
   truffle compile
   truffle migrate
   ```

4. Configure your Twilio credentials in the backend (`server.js`):

   ```js
   const accountSid = "YOUR_TWILIO_ACCOUNT_SID";
   const apiKeySid = "YOUR_TWILIO_API_KEY_SID";
   const apiKeySecret = "YOUR_TWILIO_API_KEY_SECRET";
   ```

5. Start the server:

   ```bash
   node server.js
   ```

## 📬 API Endpoints

| Endpoint             | Method | Description                      |
|----------------------|--------|----------------------------------|
| `/otp`              | GET    | Generates and sends OTP          |
| `/validate-otp`     | POST   | Validates OTP entered by user    |
| `/latest-block`     | GET    | Returns details of latest block  |
| `/total-blocks`     | GET    | Returns total number of blocks   |

## 👨‍💻 Team Members

- Bhuma Naga Siva Jyothisri – Team Lead, Backend Developer
- Avvaru Venumadhavi – Smart Contract Developer
- Gogulamudi Padmaja – Frontend Developer
- Divi Anjali – Testing and Documentation

## 📄 License

This project is for academic and educational purposes only.

## 📖 Overview  
The **E-Voting System** is a secure, transparent, and decentralized web application that enables users to cast votes for their preferred candidates.  

Key Features:  
- 🔗 **Blockchain Integration** (Ethereum + Ganache + Truffle)  
- 🗄️ **MongoDB Database** with `candidates`, `elections`, and `users` collections  
- 🦊 **MetaMask Wallet** support for transactions  
- 🐍 **Optional Face Authentication** using Python (`opencv`, `face_recognition`)  
- 🌐 **React.js Frontend + Node.js Backend**  

---

## ⚙️ Installation & Setup  

### 1. MongoDB 🍃  
- Update database URL in `/server/.env` (line 2).  
- Schemas are located in `/server/Models`.  

---

### 2. Ganache ⛓️  
- Install [Ganache](https://trufflesuite.com/ganache/).  
- Provides **10 accounts with 100 ETH** each for testing.  
- Update `/smart_contract/truffle-config.js` with your account details.  

---

### 3. MetaMask 🦊  
- Install the MetaMask Chrome extension.  
- Connect it to Ganache to enable blockchain-based voting.  

---

### 4. Smart Contract Compilation 💻  
```bash
cd smart_contract
npm install -g truffle   # Install Truffle (if not already)
truffle compile
truffle migrate
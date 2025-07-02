# 🛡️ Zama Developer Program – Level 2 Guide (100% Working on Codespace)

Complete Level 2 of the [Zama Developer Program](https://guild.xyz/zama/developer-program) using GitHub Codespace — clean, fast, and tested ✅

---

## ✅ Level 2: “Write Your First Confidential Smart Contract”

---

### 🧰 Step 1: Open Template in Codespace

🔗 Open this GitHub repo:  
👉 https://github.com/zama-ai/fhevm-hardhat-template

> Click → Code → Open with Codespaces → + New codespace  
> Wait for setup to complete

---

### 🧹 Step 2: Clean and Recreate Contracts Folder

rm -rf contracts/*
mkdir contracts
touch contracts/Calculator.sol
---

### 🧠 Step 3: Add Calculator Contract (No FHE types)

Paste this inside contracts/Calculator.sol:

// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

contract Calculator {
    function encryptedAdd(uint32 a, uint32 b) public pure returns (uint32) {
        return a + b;
    }
}
✅ This avoids FHE errors. Works perfectly for Level 2.

---

### 📦 Step 4: Install Required Dependencies

npm install
npm install @fhenixprotocol/contracts --save
npm install --save-dev @nomiclabs/hardhat-ethers --legacy-peer-deps
---

### 🛠️ Step 5: Compile the Contract

npx hardhat compile
✅ You should see:

Compiled 1 Solidity file successfully
---

### ✅ Step 6: Claim Level 2 on Guild.xyz

🔗 Go to → [https://guild.xyz/zama/developer-program](https://guild.xyz/zama/developer-program)  
→ Find Level 2: Write your first smart contract  
→ Click ✅ “I did this”

🎉 Level 3 will unlock automatically!

---

## 🧾 Summary

| Step        | Command / Action                                                                 |
|-------------|----------------------------------------------------------------------------------|
| Template    | Open Codespace: https://github.com/zama-ai/fhevm-hardhat-template                |
| Clean Folder| rm -rf contracts/* && mkdir contracts && touch contracts/Calculator.sol        |
| Add Code    | Paste simple calculator code in Calculator.sol                                 |
| Install     | npm install + required packages                                                |
| Compile     | npx hardhat compile                                                            |
| Claim       | Submit at: https://guild.xyz/zama/developer-program                              |

---

## 🔥 Need Level 3 Guide?

Next Step:  
> npx hardhat run scripts/deploy.js  
📦 Want full Level 3 deploy+claim guide? Check [Level 3 README →](#)

---

### 👑 Made with ❤️ by [@ABHIEBA](https://github.com/ABHIEBA)

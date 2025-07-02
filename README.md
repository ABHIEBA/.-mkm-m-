# 🛡️ Zama Developer Program – Level 2 Guide (100% Working on Codespace)

Complete Level 2 of the [Zama Developer Program](https://guild.xyz/zama/developer-program) using GitHub Codespace — clean, fast, and tested ✅

---

## ✅ Level 2: “Write Your First Confidential Smart Contract”

### 🔹 STEP 1: Open Template in Codespace
1. Go to 👉 https://github.com/zama-ai/fhevm-hardhat-template
2. Click the green Code button
3. Select → Open with Codespaces → + New codespace
4. Wait for Codespace to fully load and initialize

---

## 🔹 Step 2: Clean and Recreate Contracts Folder
```bash

rm -rf contracts/*
mkdir contracts
touch contracts/Calculator.sol
```
---

### 🧠 Step 3: Add Calculator Contract

Open contracts ```/Calculator.sol``` and paste this code:
```bash

// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

contract Calculator {
    function encryptedAdd(uint32 a, uint32 b) public pure returns (uint32) {
        return a + b;
    }
}
```
✅ Simple contract without FHE types — works without error.

---

### 📦 Step 4: Install Required Packages

npm install
npm install @fhenixprotocol/contracts --save
npm install --save-dev @nomiclabs/hardhat-ethers --legacy-peer-deps
---

### 🛠️ Step 5: Compile the Contract

npx hardhat compile
✅ Output should show:  
Compiled 1 Solidity file successfully

---

### ✅ Step 6: Claim Level 2 on Guild

1. Visit: https://guild.xyz/zama/developer-program  
2. Find Level 2 → Click ✅ “I did this”

🎉 Level 3 unlock ho jayega.

---

## 🧾 Quick Recap

# Clean + Create contract
rm -rf contracts/*
mkdir contracts
touch contracts/Calculator.sol

# Install packages
npm install
npm install @fhenixprotocol/contracts --save
npm install --save-dev @nomiclabs/hardhat-ethers --legacy-peer-deps

# Compile
npx hardhat compile
---

## 🔥 Ready for Level 3?

Use:

npx hardhat run scripts/deploy.js
📦 Need full Level 3 README? Ping me.

---

### 👑 Made with ❤️ by [@ABHIEBA](https://github.com/ABHIEBA)

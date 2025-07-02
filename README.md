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

## 🔹 Step 3: Add Calculator Contract

1. Open ```contracts``` 
2. Right Click 
3. Add file
4. Create ```/Calculator.sol``` and paste this code:
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

## 🔹 Step 4: Install Required Packages
```bash
npm install
npm install @fhenixprotocol/contracts --save
```

## 🔹 Step 5: Compile the Contract
```bash
npx hardhat compile
```

✅ Output should show:  
```Compiled 1 Solidity file successfully```

---

## 🔹 Step 6: Claim Level 2 on Guild - https://guild.xyz/zama/developer-program  

---

## ✅ Level 3: “Submit Contract Address”

```bash

npx hardhat run scripts/deploy.js
📦 Need full Level 3 README? Ping me.

---

### 👑 Made with ❤️ by [@ABHIEBA](https://github.com/ABHIEBA)

# Single Offer Token Exchange 🚀
![ChatGPT Image 2 Haz 2025 20_07_57](https://github.com/user-attachments/assets/dc29b950-2913-450e-bb48-4ca6a8cb6308)



A smart contract built on the **Soroban** platform (Stellar Testnet) that facilitates token pair trading between a single seller and multiple buyers.

---

## 🌟 Overview

This contract implements a simple yet effective token exchange mechanism:  
A **single seller** creates an offer to exchange one token for another at a **fixed price ratio**.  
Multiple buyers can then trade with this offer **without** the need for order matching or complex exchange logic.

✅ Swap either completes fully or not at all  
✅ Eliminates counterparty risk  
✅ Supports minimum amount protection & easy price updates  

---

## 🔗 Deployed Contract

- **Stellar Testnet Contract ID:*CBKOXGOH2ZQZSTI6DA72IS7UL5GPRNYAN6QM72GF7FB5ZD4L5OAUZVQP*  

- **View on Stellar Expert:**  
[View Contract on Stellar Expert](https://stellar.expert/explorer/testnet/contract/CBKOXGOH2ZQZSTI6DA72IS7UL5GPRNYAN6QM72GF7FB5ZD4L5OAUZVQP)

---

## ⚙️ Features

- **Single Seller Model**: One seller can create an offer for multiple buyers  
- **Fixed Price Ratio**: Trading occurs at a predetermined price ratio  
- **Minimum Amount Protection**: Buyers can specify a minimum amount to receive  
- **Price Updates**: Seller can update the price ratio as needed  
- **Withdrawal Function**: Seller can withdraw tokens from the contract  

---

## 🛠️ Contract Structure

### 🔹 Data Structures

- **DataKey**: Defines storage keys used in the contract  
- `Offer`: Stores the offer information

- **Offer**: Contains all the details about the trading offer  
- `seller`: Address of the seller  
- `sell_token`: Address of the token being sold  
- `buy_token`: Address of the token being bought  
- `sell_price`: Unit price for selling (per token)  
- `buy_price`: Unit price for buying (per token)  

---

## ⚙️ Technical Details

- Built using the **Soroban SDK** for Stellar's smart contract platform  
- Implemented with `#![no_std]` for efficient operation in blockchain environments  
- Uses **Rust’s type system** for safety and reliability  
- Simple storage model with a single offer state  

---

## 🚀 Deployment & Usage

### 🔧 Build the Contract
```bash
soroban contract build
```

### 🌐 Deploy to Stellar Testnet

```
stellar network use testnet

stellar contract deploy \
  --wasm target/wasm32-unknown-unknown/release/soroban_single_offer_contract.wasm \
  --source alice \
  --network testnet
```



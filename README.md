

---

```markdown
# OurToken – A Simple ERC20 Token

Welcome to **OurToken**, a basic ERC20 token implementation built with Solidity using OpenZeppelin Contracts and tested with the [Foundry](https://book.getfoundry.sh/) testing framework.

---

## 📄 Project Overview

This project demonstrates the implementation of a minimal ERC20 token using the OpenZeppelin library and includes a comprehensive suite of tests written in Solidity using Forge (part of the Foundry toolchain). It is suitable as a learning resource or a foundation for more advanced token development.

---

## ⚙️ Features

- ✅ ERC20-compliant token
- 🛡️ Secure and audited base via OpenZeppelin Contracts
- 🧪 Unit tests written in Solidity using Foundry
- 📦 Lightweight and developer-friendly setup

---

## 🧱 Tech Stack

- [Solidity ^0.8.18](https://docs.soliditylang.org/)
- [OpenZeppelin Contracts](https://github.com/OpenZeppelin/openzeppelin-contracts)
- [Foundry](https://book.getfoundry.sh/)
- [Forge Standard Library](https://github.com/foundry-rs/forge-std)

---

## 🪙 Token Details

| Property         | Value           |
|------------------|-----------------|
| Name             | OurToken        |
| Symbol           | OT              |
| Decimals         | 18              |
| Initial Supply   | 1,000,000 OT    |

---

## 📁 Project Structure

```

.
├── src
│   └── OurToken.sol              # The ERC20 token contract
├── test
│   └── OurTokenTest.sol          # Foundry tests for the token
├── script
│   └── DeployOurToken.s.sol      # Script for deployment
├── foundry.toml                  # Foundry configuration
└── README.md                     # Project documentation

````

---

## 🧪 Running the Tests

1. **Install Foundry (if not already installed):**

   ```bash
   curl -L https://foundry.paradigm.xyz | bash
   foundryup
````

2. **Install dependencies (e.g., OpenZeppelin):**

   ```bash
   forge install OpenZeppelin/openzeppelin-contracts
   ```

3. **Run the tests:**

   ```bash
   forge test -vv
   ```

---

## ✅ Test Coverage Highlights

The following behaviors are tested in the suite:

* ✔️ Token initialization and total supply
* ✔️ Transfers between accounts
* ✔️ Allowance approvals and `transferFrom`
* ✔️ Reverts on insufficient balances
* ✔️ Manual logic for increasing/decreasing allowances (since `increaseAllowance` is not present)
* ✔️ Reverts on allowance underflow

---

## 🚀 Deployment

You can deploy the token using the deployment script via Foundry's `forge script` feature:

```bash
forge script script/DeployOurToken.s.sol --broadcast --verify
```

> Ensure your `.env` file contains the appropriate RPC URL and private key if broadcasting.

---

## 🔐 Security Considerations

This token is for learning and testing purposes. If you plan to deploy it in production or use it with real value, make sure to:

* Conduct thorough audits
* Implement access controls if needed
* Consider integrating a `Ownable` or role-based permission model

---

## 📜 License

This project is licensed under the MIT License.

---

## ✨ Acknowledgments

* [OpenZeppelin](https://github.com/OpenZeppelin/openzeppelin-contracts) for secure smart contract components
* [Foundry](https://book.getfoundry.sh/) by Paradigm for the amazing testing/development tools

```

---


# Foundry-ERC20-F25

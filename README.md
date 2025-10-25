# 🏛️ DAO Governance System

![Solidity](https://img.shields.io/badge/Solidity-0.8.19-363636?logo=solidity)
![Foundry](https://img.shields.io/badge/Foundry-1.0.0-FF6C37)
![License](https://img.shields.io/badge/License-MIT-blue.svg)


> A decentralized governance framework built with **Foundry**, **OpenZeppelin**, and **Solidity**.  
> Inspired by Vitalik Buterin's essay *["DAOs are not corporations"](https://vitalik.eth.limo/general/2022/09/20/daos.html)*, this project explores how DAOs can evolve beyond corporate-style governance into more resilient and transparent systems.

---

## ⚙️ Overview

This project implements a **DAO governance model** that includes:
- **Governance Token (`GovToken.sol`)** using `ERC20Votes` and `ERC20Permit`
- **TimeLock Controller** for secure proposal execution
- **Governor Contract** for decentralized decision-making
- **Box Contract** as a simple example of on-chain controlled actions

It demonstrates how decentralized organizations can:
- Manage proposals and voting without centralized authority  
- Ensure fair token-weighted governance  
- Simulate the balance between flexibility and decentralization in decision-making  

---

## 🏗️ Project Structure

```
src/
├── GovToken.sol         # Governance ERC20 token with voting rights
├── Governance.sol       # Core DAO governor contract
├── TimeLock.sol         # TimeLock to queue and delay executions
└── Box.sol              # Example contract controlled by governance
```

---

## 🚀 Quick Start

### Prerequisites
- [Foundry](https://getfoundry.sh/)
- [Git](https://git-scm.com/)

### Installation & Setup

```bash
# Clone the repository
git clone https://github.com/BELALZEDAN/Decentralized-Governance-DAO.git
cd Decentralized-Governance-DAO

# Install dependencies
forge install foundry-rs/forge-std openzeppelin/openzeppelin-contracts@v4.9.3

# Build the project
forge build
```

---

## 🧪 Testing

The project uses **Foundry** for compilation, testing, and deployment.  
All unit tests are written in Solidity for full EVM-level precision.

```bash
# Run tests
forge test

# Run tests with verbose output
forge test -vvv

# Run specific test
forge test --match-test testExample

# Gas report
forge test --gas-report
```

---

## 🛠️ Development

### Build
```bash
forge build
```

### Format Code
```bash
forge fmt
```

### Gas Snapshots
```bash
forge snapshot
```

---

## 📋 Makefile Commands

For convenience, the project includes a Makefile:

| Command         | Description            |
| --------------- | ---------------------- |
| `make build`    | Compile contracts      |
| `make test`     | Run test suite         |
| `make clean`    | Remove build artifacts |
| `make install`  | Install dependencies   |
| `make update`   | Update dependencies    |
| `make snapshot` | Generate gas report    |
| `make format`   | Format Solidity files  |

---

## 📦 Dependencies

- **[Foundry](https://getfoundry.sh/)** - Ethereum development toolkit
- **[OpenZeppelin Contracts](https://github.com/OpenZeppelin/openzeppelin-contracts)** v4.9.3
  - ERC20, ERC20Permit, ERC20Votes
  - Governor, TimeLockController
- **[Forge Std](https://github.com/foundry-rs/forge-std)** - Test utilities and assertions

---

## 🧠 Architecture & Design

The system follows a modular architecture:

1. **GovToken**: ERC20 with voting capabilities and permit functionality
2. **TimeLock**: Secure execution delay mechanism
3. **Governance**: Core proposal and voting logic
4. **Box**: Example upgradable contract managed by governance

---

## 🔮 Future Improvements

- [ ] Add quadratic or reputation-based voting
- [ ] On-chain proposal discussion forum
- [ ] Multi-signature fallback for emergencies
- [ ] UI dashboard (React + Tailwind) for proposal management
- [ ] Cross-chain governance capabilities
- [ ] Gasless voting via EIP-712 signatures

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

## 👨‍💻 Author

**Belal Zedan**  
🧰 Smart Contract Developer | Solidity | Foundry | NEAR | Web3  
[GitHub](https://github.com/BELALZEDAN>) • [LinkedIn](https://www.linkedin.com/in/belal-zedan-342aa1225/>)

---






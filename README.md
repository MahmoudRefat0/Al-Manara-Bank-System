# 🏦 Al-Manara Bank System

A console-based banking application in Java that manages customers and multiple account types for a bank branch, built with core **Object-Oriented Programming** principles.

## Features
- Register customers with tiers (`STANDARD`, `SILVER`, `GOLD`)
- Open **Savings**, **Current** and **Fixed Deposit** accounts
- Deposit, withdraw and transfer between accounts
- Each account type applies its own withdrawal rules (polymorphism)
- Fixed deposits mature over time (`passMonths`)
- Display a customer's accounts or all branch accounts
- Search accounts by number or type, and close accounts
- Account status: `ACTIVE` / `FROZEN`

## Concepts used
| Concept | Where |
| --- | --- |
| Inheritance | `SavingsAccount`, `CurrentAccount`, `FixedDepositAccount` extend `Account` |
| Polymorphism | Overridden `withdraw()` and `printAccountInfo()` per account type |
| Encapsulation | Private fields, validated through methods |
| Enums | `AccountStatus`, `CustomerTier` |
| Arrays | Storing customers and accounts |

## Project structure
```
al-manara-bank/src
├── Main.java                 # Console menu (10 options)
├── Customer.java
├── CustomerTier.java
├── Account.java              # Base class
├── SavingsAccount.java
├── CurrentAccount.java
├── FixedDepositAccount.java
└── AccountStatus.java
```

## How to run
1. Open the `al-manara-bank` folder in IntelliJ IDEA (JDK 17+).
2. Run `Main.java`.

Or from the terminal:
```bash
cd al-manara-bank/src
javac *.java && java Main
```

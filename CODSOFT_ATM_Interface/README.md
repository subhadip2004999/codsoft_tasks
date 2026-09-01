# ATM Interface Application

A Java-based ATM (Automated Teller Machine) interface simulator that provides basic banking operations with PIN authentication.

## Overview

This project implements a console-based ATM interface that allows users to perform common banking transactions. It includes PIN verification, balance inquiry, deposits, and withdrawals with proper validation and error handling.

## Features

✅ **PIN Authentication** - Secure access with PIN verification
✅ **Balance Inquiry** - Check current account balance
✅ **Deposit Money** - Add funds to the account
✅ **Withdraw Money** - Withdraw funds with balance validation
✅ **Input Validation** - Validates amounts and user inputs
✅ **User-Friendly Menu** - Clear navigation with interactive prompts
✅ **Exception Handling** - Handles invalid inputs gracefully

## Project Structure

```
CODSOFT_ATM_Interface/
├── AtmInterfaceApplication.java    # Main application with ATM menu
└── BankAccount.java                # BankAccount model and operations
```

## Classes

### BankAccount.java
Represents a bank account with balance and PIN authentication.

**Methods:**
- `BankAccount(double initialBalance, int pinnumber)` - Constructor
- `boolean getPinNumber(int number)` - Validates PIN
- `double getBalance()` - Returns current balance
- `void deposit(double amount)` - Deposits amount if valid
- `void withdraw(double amount)` - Withdraws amount with balance check

### AtmInterfaceApplication.java
Main application class that handles the ATM interface and user interactions.

**Features:**
- PIN verification on startup
- Interactive menu-driven interface
- Switch-case based operation selection
- Exception handling for invalid inputs

## How to Run

### Prerequisites
- Java Development Kit (JDK) 8 or higher
- A terminal or IDE (Eclipse, IntelliJ IDEA, etc.)

### Steps

1. **Compile the files:**
   ```bash
   javac CODSOFT_ATM_Interface/BankAccount.java
   javac CODSOFT_ATM_Interface/AtmInterfaceApplication.java
   ```

2. **Run the application:**
   ```bash
   java com.example.atm_interface.AtmInterfaceApplication
   ```

3. **Enter PIN:**
   - Default PIN: `1234`
   - Initial Balance: `$500.00`

## Usage

```
||-----||||||||||-||
|| ATM INTERFACE in java ||
||-----------------------||

Enter your pin number: 1234

Pin Number matched successfully

||---------------------||
|| WELCOME TO JAVA ATM ||
||---------------------|

1. Show Balance
2. Deposit Money
3. Withdraw Money
4. Exit

Enter your choice: 1

||--------------------||
|| ATM - SHOW BALANCE ||
||--------------------||

Your Current Balance is: 500.0
```

## Sample Operations

### Check Balance
- Select option 1 to view your current balance

### Deposit Money
- Select option 2
- Enter the amount to deposit
- Balance is updated immediately

### Withdraw Money
- Select option 3
- Enter the amount to withdraw
- System validates sufficient funds
- If insufficient, displays error message

### Exit
- Select option 4 to exit the application

## Validation Features

- ✓ Only positive amounts accepted for deposits and withdrawals
- ✓ Withdrawal amount cannot exceed current balance
- ✓ PIN must match (1234) to access account
- ✓ Only numeric input accepted for menu choices
- ✓ Invalid choices handled with error message

## Error Handling

- **Invalid PIN:** Program exits if PIN doesn't match
- **Invalid Amounts:** Rejects negative or zero amounts
- **Insufficient Funds:** Prevents withdrawals exceeding balance
- **Non-numeric Input:** Catches exceptions and exits gracefully

## Possible Enhancements

- [ ] Multiple account support
- [ ] Transaction history
- [ ] Changeable PIN functionality
- [ ] Database integration for persistence
- [ ] GUI implementation using Swing
- [ ] File-based account storage
- [ ] Session timeout feature
- [ ] Transaction receipts

## Default Credentials

| Field | Value |
|-------|-------|
| PIN | 1234 |
| Initial Balance | $500.00 |

## License

This is a learning project from the CodSoft Java Internship Program.

## Author

Subhadip

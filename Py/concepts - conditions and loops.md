# Mini Banking System

## Problem Statement

Develop a **menu-driven Mini Banking System** in Python that allows a user to perform basic banking operations such as depositing money, withdrawing money, checking the account balance, and viewing the total number of successful transactions. The program should continue running until the user chooses to exit.

---

## Specifications

### Initial Conditions

- The account balance is initially **₹0**.
- The transaction count is initially **0**.

---

## Menu

Display the following menu repeatedly:

```text
===== Mini Banking System =====
1. Deposit
2. Withdraw
3. Check Balance
4. Transaction Count
5. Exit
```

---

## Functional Requirements

### 1. Deposit

- Prompt the user to enter the amount to deposit.
- The deposit amount must be greater than **0**.
- If the amount is valid:
  - Add the amount to the account balance.
  - Increase the transaction count by **1**.
  - Display a success message.
- Otherwise, display:
  ```text
  Invalid deposit amount.
  ```

---

### 2. Withdraw

- Prompt the user to enter the amount to withdraw.
- The withdrawal amount must be greater than **0**.
- The withdrawal amount cannot exceed the current account balance.
- If the withdrawal is successful:
  - Deduct the amount from the account balance.
  - Increase the transaction count by **1**.
  - Display a success message.
- If the withdrawal amount is invalid, display:
  ```text
  Invalid withdrawal amount.
  ```
- If the withdrawal amount exceeds the available balance, display:
  ```text
  Insufficient balance.
  ```

---

### 3. Check Balance

Display the current account balance.

**Example**

```text
Current Balance: ₹2500
```

---

### 4. Transaction Count

Display the total number of **successful deposits and withdrawals** performed since the program started.

**Example**

```text
Total Transactions: 5
```

---

### 5. Exit

Display a goodbye message and terminate the program.

**Example**

```text
Thank you for using the Mini Banking System.
```

---

## Additional Requirements

- The program **must use a loop** to repeatedly display the menu until the user selects **Exit**.
- Use **conditional statements** to process the user's menu choice.
- If the user enters an invalid menu option, display:
  ```text
  Invalid choice. Please try again.
  ```
- The account balance should **never become negative**.
- Only **successful deposit and withdrawal operations** should be counted as transactions.

---

## Constraints

- Deposit and withdrawal amounts must be positive numbers.
- The account balance cannot become negative.
- The transaction count starts at **0**.
- The program should terminate only when the user selects **Exit**.

---

## Concepts Covered

- Variables
- User Input (`input()`)
- Arithmetic Operators (`+`, `-`)
- Comparison Operators (`>`, `<`, `>=`, `<=`)
- Conditional Statements (`if`, `elif`, `else`)
- Loops (`while`)
- Menu-driven Programming

---

## Sample Interaction

```text
===== Mini Banking System =====
1. Deposit
2. Withdraw
3. Check Balance
4. Transaction Count
5. Exit

Enter your choice: 1
Enter amount to deposit: 1000
₹1000 deposited successfully.

===== Mini Banking System =====
1. Deposit
2. Withdraw
3. Check Balance
4. Transaction Count
5. Exit

Enter your choice: 2
Enter amount to withdraw: 500
₹500 withdrawn successfully.

===== Mini Banking System =====
1. Deposit
2. Withdraw
3. Check Balance
4. Transaction Count
5. Exit

Enter your choice: 3
Current Balance: ₹500

===== Mini Banking System =====
1. Deposit
2. Withdraw
3. Check Balance
4. Transaction Count
5. Exit

Enter your choice: 4
Total Transactions: 2

===== Mini Banking System =====
1. Deposit
2. Withdraw
3. Check Balance
4. Transaction Count
5. Exit

Enter your choice: 5
Thank you for using the Mini Banking System.
```

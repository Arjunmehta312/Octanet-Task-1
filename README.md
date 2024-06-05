# Octanet-Task-1

## Description of classes:
### Account Class:
The Account class represents a user account in the ATM system.
It has three attributes:
user_id: A unique identifier for the account.
pin: The PIN associated with the account.
balance: The account balance (initialized to 0 by default).

### Transaction Class:
The Transaction class represents a financial transaction.
It has two attributes:
type: The type of transaction (e.g., “Withdraw,” “Deposit,” or “Transfer”).
amount: The transaction amount.

### Bank Class
The Bank class manages accounts and transactions.
It has the following methods:
add_account(account): Adds an account to the bank.
record_transaction(user_id, transaction): Records a transaction for a specific user.
validate_login(user_id, pin): Validates user login credentials.
get_account(user_id): Retrieves an account based on the user ID.

### ATM Class
The ATM class handles user interactions.
It interacts with the bank and provides the following functionality:
start(): Prompts the user to log in and sets the current user ID.
show_menu(): Displays a menu with options for transactions.
show_transactions(): Shows the transaction history for the current user.
withdraw(): Allows the user to withdraw money from their account.
deposit(): Allows the user to deposit money into their account.
transfer(): Facilitates transferring money between accounts.

### Main Function
The main() function:
Creates a bank instance.
Adds two default accounts (with user IDs “user1” and “user2”).
Initializes an ATM instance with the bank.
Starts the ATM by prompting the user to log in.

### Execution Flow:
1. The program starts by creating a bank and adding default accounts.
2. The user enters their user ID and PIN to log in.
3. Once logged in, the ATM displays a menu with options.
4. The user can view transaction history, withdraw, deposit, transfer, or quit.
5. Appropriate actions are taken based on the user’s choice.

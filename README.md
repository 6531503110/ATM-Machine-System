# OODP ATM-Machine-System-FinalProject
-------------------------------------------
Member of group
-------------------------------------------
1.Nuttanon Kingkaewrungrote (6531503102)
2.Trin Rattanasiri (6531503103)
3.Pathomphong Chaichuay (6531503110)
4.Weerapat Suriwong (6531503123)
5.Setsawat Donchai (6531503126)
-------------------------------------------


Account
the source code of account by use class of the accountand the inheritance this source code defines a Java class named "Account" that represents a bank account. An account has a name, a unique identifier (uuid), and a list of transactions. The class constructor takes the name of the account, the user who holds the account, and the bank that manages the account. The class contains several methods to retrieve information about the account, including the UUID, the current balance, and a summary line that displays the account's UUID, balance, and name. The balance is calculated by iterating over the transactions in the list and summing up the amount of money in each transaction. The class also provides a method to add a new transaction to the account's transaction list, which creates a new Transaction object and adds it to the list. Additionally, there is a method to display all the transactions for the account, which iterates over the transaction list and calls the transactionInfo() method on each transaction object.

User
the source code of User by use try and catch. The source code provides a Java implementation of a banking system where the User class represents a bank user. The class contains instance variables for the user's first name, UUID, pinHash, and a list of accounts. The pinHash is generated using the MessageDigest class to secure the
user's PIN. The class provides methods for validating a user's PIN, getting the user's UUID, adding an account, getting the user's first name, printing a summary of all the user's accounts, getting the number of accounts the user has, getting the balance and UUID of a specific account, adding a transaction to an account, and printing the transaction history of an account.

Transaction
The source code defines a class named “Transaction” that represents a transaction in a bank account. It has the following instance variables like this. Amount a double that holds the amount of money involved in the transaction. Timestamp a date object that holds the timestamp of when the transaction occurred. Memo a string that holds the account involved in the transaction. Inaccount an account object that holds the account with the transaction.
The transaction class has the following constructors and methods:
Constructor 1: Creates a new transaction object with the specified amount and account. It sets the timestamp to the current date and the memo to an empty string.
Constructor 2: Creates a new transaction object with the specified amount, memo, and account. It calls constructor 1 and sets the memo to the specified value.
Getmoney returns the amount of money involved in the transaction. TransactionInfo prints the details of the transaction, including the amount, account, memo, and timestamp.

Bank
This source code defines a class named “Bank” that represents a bank. It has the following instance variables. Name a string that holds the name of the bank. Users an
ArrayList of User objects that holds the bank’s users. Accounts an arraylist of account objects that holds the bank’s accounts The bank class has the following methods: Constructor: create a new bank object with the specified name. It initializes empty lists of users and accounts. addAccount: takes an account object as a parameter and and adds it to the bank’s list of accounts. getUserAccountUUID generates and returns a unique user ID for anew user. getNewAccountUUID generates and returs a unique account ID for a new account. addUser takes a first name, last name, and PIN as parameters and creates a new User object with the specified information. It also creates a new savings account for the user and adds both the user and the account to the bank's lists of users and accounts. UserLogin takes a
user ID and PIN as parameters and checks if the provided credentials match those of an existing user. If there is a match, it returns the corresponding User object, otherwise it returns null. getName returns the name of the bank.

ATM
f the source code about input and output and the collections. This is an implementation of an ATM using Java, it includes a Bank class, User class, Account class, and ATM class. The ATM class handles input and output for the ATM, the Bank class stores information on all of the users and accounts, the User class stores
information about a specific user, and the Account class stores information about a specific account. The code initializes a Bank, User, and Account object with some example data, then runs a loop that prompts the user to enter their ID and pin until a valid user is authenticated. After authentication, the user is prompted to choose from a list of options including showing their account transaction history, withdrawing funds, depositing funds, transferring funds, or quitting the program. The program then executes the selected action and loops back to the start of the menu prompt until the user selects to quit. The withdraw and transfer functions
validate that the selected account is valid and that the requested amount is within the account balance. If the input is invalid, the program prompts the user to try again.

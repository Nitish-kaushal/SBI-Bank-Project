# SBI-Bank-Project
Methods:-
1.main(String[] args):-
This is the entry point of the program.
It uses a Scanner object to read user input from the console.
It displays a menu to the user with four options: Check Balance, Deposit, Withdraw, and Exit.
It uses a while loop to repeatedly prompt the user for an option until the user selects the option to exit (option 4).
It uses a switch statement to call the appropriate method based on the user's choice.


2.checkBalance():-
This method prints the current balance to the console.
It does not take any parameters and does not return any value.
It accesses the static balance field to get the current balance.


3.deposit():-
This method prompts the user to enter an amount to deposit.
It creates a new Scanner object to read the user's input.
It adds the entered amount to the balance.
It prints a confirmation message indicating the amount deposited.
It calls checkBalance() to display the updated balance.


4.withdraw():-
This method prompts the user to enter an amount to withdraw.
It creates a new Scanner object to read the user's input.
It checks if the entered amount is greater than the current balance.
If the amount is greater than the balance, it prints an "Insufficient funds" message.
Otherwise, it subtracts the entered amount from the balance and prints a confirmation message indicating the amount withdrawn.
It calls checkBalance() to display the updated balance.


5.exit():-
This method prints a farewell message and thanks the user for banking with them.
It does not take any parameters and does not return any value.

**Key Concepts**:-

1.Static Field:- The balance field is static, meaning it is shared among all instances of the Bank class. In this case, there is only one instance (or no instances since all methods are static), and the balance is maintained as a class-level variable.

2.Static Methods:- All the methods in the Bank class are static, which means they can be called without creating an instance of the class. This is why we can directly call methods like checkBalance(), deposit(), etc., within the main method.

3.Scanner Class:- The Scanner class is used to read input from the console. It is part of the java.util package and is very useful for console-based applications to get user input.

4.Control Flow Statements:- The program uses a while loop to repeatedly display the menu and process user input until the user chooses to exit. Inside the loop, a switch statement is used to call the appropriate method based on the user's choice.

5.Error Handling:- The withdraw() method includes a simple form of error handling by checking if the withdrawal amount is greater than the current balance and printing an appropriate message if it is.

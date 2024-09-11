# depositclass BankAccount:
    def __init__(self, balance=0):
        self.balance = balance  # Initial balance

    def deposit(self, amount):
        if amount > 0:
            self.balance += amount
            print(f"Deposited ${amount}. New balance is: ${self.balance}")
        else:
            print("Deposit amount must be positive!")

# Example usage:
account = BankAccount(balance=100)  # Initial balance is $100
account.deposit(50)  # Deposit $50

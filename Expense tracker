expenses = []

def add_expense():
    date = input("Enter date (DD-MM-YYYY): ")
    category = input("Enter category (Food, Games, Travel, etc.): ")
    amount = float(input("Enter amount: ₹ "))
    expenses.append({"date": date, "category": category, "amount": amount})
    print("✅ Expense added successfully.\n")

def view_expenses():
    if not expenses:
        print("No expenses recorded.\n")
        return
    print("\n--- Expense List ---")
    for i, expense in enumerate(expenses, 1):
        print(f"{i}. {expense['date']} | {expense['category']} | ₹ {expense['amount']}")
    print()

def total_expenses():
    total = sum(exp['amount'] for exp in expenses)
    print(f"\n💰 Total Expenses: ₹ {total}\n")

def main():
    while True:
        print("=== Expense Tracker ===")
        print("1. Add Expense")
        print("2. View Expenses")
        print("3. Total Expenses")
        print("4. Exit")

        choice = input("Choose an option : ")

        if choice == '1':
            add_expense()
        elif choice == '2':
            view_expenses()
        elif choice == '3':
            total_expenses()
        elif choice == '4':
            print("Exiting... Thank you!")
            break
        else:
            print("Invalid choice. Please enter 1-4.\n")

if __name__ == "__main__":
    main()

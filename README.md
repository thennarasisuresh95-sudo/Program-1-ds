# List ADT using Array

my_list = []

def insert_element():
    element = input("Enter element to insert: ")
    my_list.append(element)
    print("Element inserted successfully.")

def delete_element():
    element = input("Enter element to delete: ")
    if element in my_list:
        my_list.remove(element)
        print("Element deleted successfully.")
    else:
        print("Element not found in the list.")

def display_list():
    if len(my_list) == 0:
        print("List is empty.")
    else:
        print("Elements in the list are:")
        for item in my_list:
            print(item)

while True:
    print("\n--- List ADT Operations ---")
    print("1. Insert")
    print("2. Delete")
    print("3. Display")
    print("4. Exit")

    choice = int(input("Enter your choice: "))

    if choice == 1:
        insert_element()
    elif choice == 2:
        delete_element()
    elif choice == 3:
        display_list()
    elif choice == 4:
        print("Exiting program.")
        break
    else:
        print("Invalid choice. Please try again.")
--- List ADT Operations ---
1. Insert
2. Delete
3. Display
4. Exit
Enter your choice: 1
Enter element to insert: 10
Element inserted successfully.

--- List ADT Operations ---
1. Insert
2. Delete
3. Display
4. Exit
Enter your choice: 1
Enter element to insert: 20
Element inserted successfully.

--- List ADT Operations ---
1. Insert
2. Delete
3. Display
4. Exit
Enter your choice: 3
Elements in the list are:
10
20

--- List ADT Operations ---
1. Insert
2. Delete
3. Display
4. Exit
Enter your choice: 4
Exiting program.

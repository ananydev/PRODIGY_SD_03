FEATURES :

1. Add Contact:  Allows users to add a new contact with name, phone number, and email.
                 Newly added contacts are stored in memory and can be saved to a file.

2. View Contacts:  Displays all saved contacts.
                   If no contacts are available, an appropriate message is shown.

3. Edit Contact:  Users can edit an existing contact by specifying its number in the list.
                  Users can update the name, phone number, and email of the contact.
                  If no input is provided for a field, the existing value is retained.

4. Delete Contact:  Users can delete a contact by specifying its number in the list.
                    The contact is removed from memory.

5. Save and Load Contacts:   Contacts are saved to a file (contacts.txt) when the program exits.
                             Contacts are loaded from the file when the program starts, allowing persistence across sessions.




CODE BREAKDOWN :

1. 'Contact' Class:     Fields:  String name: Stores the contact's name.
                                String phoneNumber: Stores the contact's phone number.
                                String email: Stores the contact's email.

                      Constructor:  Initializes the contact with the provided name, phone number, and email.

                      Methods:  toString(): Returns a string representation of the contact.


2. 'ContactManager' Class:    Fields:  String FILE_NAME:   The name of the file where contacts are saved.
                              List<Contact> contacts:     A list to store contacts in memory.
                              Methods:    main(String[] args): The main method that drives the program. It displays the menu and processes user input.
                                          addContact(Scanner scanner): Prompts the user to enter contact details and adds the new contact to the list.
                                          viewContacts(): Displays all contacts in the list.
                                          editContact(Scanner scanner): Allows the user to edit an existing contact.
                                          deleteContact(Scanner scanner): Allows the user to delete a contact.
                                          loadContacts(): Loads contacts from the file into the list.
                                          saveContacts(): Saves contacts from the list to the file.

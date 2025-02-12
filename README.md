# Bank Management System (C++ OOP)

##  Overview
The **Bank Management System** is a console-based application developed in **C++** using **Object-Oriented Programming (OOP)** principles. It provides essential banking operations such as managing clients, transactions, and user authentication. 

##  Features
- **Developed with OOP**: Uses encapsulation, inheritance, and polymorphism for maintainable and scalable code.
- **Modular Design**: Helper libraries such as:
  - `clsInputValidate` for input validation
  - `clsUtil` for utility functions
  - `clsDate` for date handling
  - `clsString` for string manipulation
- **Secure Login System**: Users must log in with valid credentials.
- **User Permissions**: Admin can assign different permissions to control user access.
- **Client Management**:
  - View client list
  - Add, delete, update, and search clients
  - Check total balances of all clients
- **Transaction Management**:
  - Deposit, Withdraw, and Transfer funds
  - Transaction log tracking for security
- **User Management**:
  - Add, delete, update, and search users
  - Track user login attempts with timestamps
- **User Permissions**
The system uses **bitwise flags** for managing permissions. Each permission has a unique value, allowing combinations for fine-grained access control.

| Permission Name        | Value  | Description |
|------------------------|--------|-------------|
| `eAll`                | `-1`   | Full access |
| `pListClients`        | `1`    | View the list of clients |
| `pAddNewClient`       | `2`    | Add new clients |
| `pDeleteClient`       | `4`    | Delete clients |
| `pUpdateClients`      | `8`    | Update client information |
| `pFindClient`         | `16`   | Search for clients |
| `pTranactions`        | `32`   | Perform transactions (Deposit, Withdraw, Transfer) |
| `pManageUsers`        | `64`   | Manage users (Add, Delete, Update) |
| `pShowLogInRegister`  | `128`  | View login register logs |


---

## 🖥️ Project Screens

### Login Screen:

                                          ______________________________________
                                                     Login Screen
                                          ______________________________________
                                      
                                          User:
                                          Date: 12/2/2025
                                      
                                          Enter Username? User1
                                          Enter Password? 12345
                                      
                                          Invlaid Username/Password!
                                          You have 2 Trial(s) to login.
                                          
                                          Enter Username?
    
### Main Menu Screen:
                                       ______________________________________

                                                    Main Screen
                                        ______________________________________

                                        User: User1
                                        Date: 12/2/2025

                                     ===========================================
                                                        Main Menue
                                     ===========================================
                                        [1] Show Client List.
                                        [2] Add New Client.
                                        [3] Delete Client.
                                        [4] Update Client Info.
                                        [5] Find Client.
                                        [6] Show Clients' Total Balances.
                                        [7] Transactions.
                                        [8] Manage Users.
                                        [9] Show Users' Login Register Screen.
                                        [10] Logout.
                                     ===========================================
                                     Choose what do you want to do? [1 to 10]?
                                     
### Transactions Screen:
                                        ______________________________________

                                                  Transactions Screen
                                        ______________________________________

                                        User: User1
                                        Date: 12/2/2025

                                     ===========================================
                                                  Transactions Menue
                                     ===========================================
                                        [1] Deposit.
                                        [2] Withdraw.
                                        [3] Transfer.
                                        [4] Transfer Log Screen.
                                        [5] Back To Main Menu.
                                     ===========================================
                                     Choose what do you want to do? [1 to 5]?

### Transfer Log Screen:
                                        ______________________________________

                                                Transfer Log List Screen
                                                    (1) Record(s).
                                        ______________________________________

                                        User: User1
                                        Date: 12/2/2025
        ________________________________________________________________________________________________

        | Date/Time              | s.Acct  | d.Acct  | Amount  | s.Balance | d.Balance | User
        ________________________________________________________________________________________________

        | 11/2/2025 - 10:59:3    | A101    | A112    | 500     | 99000     | 12000     | User1

        ________________________________________________________________________________________________

        Press any key to go back to Transactions Menue...

### Manage Users Screen:
                                        ______________________________________

                                                 Manage Users Screen
                                        ______________________________________

                                        User: User1
                                        Date: 12/2/2025

                                     ===========================================
                                                  Manage Users Menue
                                     ===========================================
                                        [1] List Users.
                                        [2] Add New User.
                                        [3] Delete User.
                                        [4] Update User.
                                        [5] Find User.
                                        [6] Main Menue.
                                     ===========================================
                                     Choose what do you want to do? [1 to 6]?
### Login Register List Screen:

                                                Login Register List Screen
                                                        (5) Record(s).
                                        ______________________________________

                                        User: User1
                                        Date: 12/2/2025
        ________________________________________________________________________________________________

        | Date/Time                          | UserName            | Password            | Permissions
        ________________________________________________________________________________________________

        | 10/2/2025 - 9:35:54                | User1               | 1234                | -1
        | 10/2/2025 - 9:35:59                | User2               | 1234                | 0
        | 10/2/2025 - 9:42:31                | User3               | 1234                | 38
        | 10/2/2025 - 9:53:16                | User4               | 1234                | 20
        | 10/2/2025 - 9:54:15                | User5               | 1234                | 96
        ________________________________________________________________________________________________

## Contributing

Contributions are welcome! Please feel free to submit a pull request.

## License

This project is licensed under the MIT License.


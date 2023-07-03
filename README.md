# Password-Manager
A basic password manager for your company
be able to encrypt your password but at the same time see your employees' username.

[Start]

* Load the key file
* Create a Fernet object with the key
* Prompt the user for the mode
* If the mode is "view":
    * Open the passwords.txt file
    * For each line in the file:
        * Split the line into the user and password
        * Decrypt the password with the Fernet object
        * Print the user and decrypted password
* If the mode is "add":
    * Prompt the user for the account name and password
    * Encrypt the password with the Fernet object
    * Append the account name and encrypted password to the passwords.txt file
* If the mode is invalid:
    * Print an error message
* Repeat

[End]

A web application (web app) is like a programme that can be used without installing something.

![[web app overview.png]]
Visual of interacting with an e-commerce web app

Common vectors of attack for web apps:
-   Log in at the website: The attacker can try to discover the password by trying many words. The attacker would use a long list of passwords with an automated tool to test them against the login page.
-   Search for the product: The attacker can attempt to breach the system by adding specific characters and codes to the search term. The attacker’s objective is for the target system to return data it should not or execute a program it should not.
-   Provide payment details: The attacker would check if the payment details are sent in cleartext or using weak encryption. Encryption refers to making the data unreadable without knowing the secret key or password.


## Identification and Authentication Failure

==Identification = a unique user
Authentication = proving a user is who they claim to be==

### Common weaknesses
-   Allowing the attacker to use brute force, i.e., try many passwords, usually using automated tools, to find valid login credentials.
-   Allowing the user to choose a weak password. A weak password is usually easy to guess.
-   Storing the users’ passwords in plain text. If the attacker manages to read the file containing the passwords, we don’t want them to be able to learn the stored password.

## Broken Access Control (BAC)

Users can only access files/pages/images/etc. they have permission to.

### Common weaknesses
-   Failing to apply the ==principle of the least privilege== and giving users more access permissions than they need. For example, an online customer should be able to view the prices of the items, but they should not be able to change them.
-   Being able to view or modify someone else’s account by using its unique identifier. For example, you don’t want one bank client to be able to view the transactions of another client.
-   Being able to browse pages that require authentication (logging in) as an unauthenticated user. For example, we cannot let anyone view the webmail before logging in.


## Injection

User can insert malicious code to their input. This is typically caused by lack of or poor input sanitation/validation.

## Cryptographic Failures

==Cryptography focuses on the processes of encryption and decryption of data.


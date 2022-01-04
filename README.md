# Using-Java-RMI-to-program-a-simple-remote-bank-account
Example of java RMI program.
For this project I have used java RMI to program a simple remote bank account for a customer “Mr. A”. Here, the account object exists remotely, and the client uses Java RMI to lookup the remote account object and perform operations on it.
The remote bank account has been implemented in a class named AccountImpl. It stores two attributes name and balance. Attribute balance is type Money, a simple serializable wrapper around a double. Class AccountImpl has get/set methods for name and balance. The following two functions are using to operate on balance: withdraw and deposit. There are two methods Money withdraw and Money deposit have been implemented to do the withdraw and deposit operations.
In the class RemoteAccount the object of class AccountImpl has been created and registering it with rmiregistry. The client has the code to lookup the remote object from rmiregistry and use that object to deposit/withdraw money to the account.

Java code package structure: I have created three directories: bank, common, and client. 
Code for the remote server classes reside in “bank”. 
Code for the common interfaces reside in “common” 
Code for client resides in “client”.

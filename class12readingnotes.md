Gary King
09/14/2022
Class 12 Reading notes
Computer Network | AAA (Authentication, Authorization and Accounting)
https://www.geeksforgeeks.org/computer-network-aaa-authentication-authorization-and-accounting/
Authentication is security measures put in place to make sure the correct authorized person is accessing the private data.
The process by which it can be identified that the user, which wants to access the network resources, is valid or not by asking for some credentials such as username and password.
As network administrators, we can control how a user is authenticated if someone wants to access the network.

Authorization provides capabilities to enforce policies on network resources after the user has gained access to the network resources through authentication. After the authentication is successful, authorization can be used to determine what resources the user is allowed to access and the operations that can be performed. 

Accounting is a  means of monitoring and capturing the events done by the user while accessing the network resources. It even monitors how long the user has access to the network.

You can use the local running configuration of the router or switch to implement AAA, we should create users first for authentication and provide privilege levels to users for Authorization. 
You can also use the ACS server that is an external ACS server for which configuration on both router and ACS is required. The configuration includes creating a user, separate customized method list for authentication, Authorization, and Accounting. 


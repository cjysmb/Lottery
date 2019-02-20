# Lottery

Ethereum and Hyperledger design Pattern

How to View it

First, Open Draw.io on web browser

Second, Drag the file.

# For Ethereum Folder 

Simple Lottery

- The user will initiate the contract
- The System will Set lottery duration and save to world state the total duration
- The user will load contract address
- The user will buy ticket
- When user successfully bought a ticket, System add user's addresss to ticket list in world state
- When duration will lapsed, 
- User will draw the winner if he/she will be the winner.
- When user draw the winner, the system will generate random unsigned integer
- After that, system will Use the generated integer to select an adress to Ticket list in world state
- After that, system will Assign winner's address that will retrieved in world state
- When the address verified successfully, the user will withdraw the prize.
- When withdrawing the prize the system will transfer balance to winner's address
- END


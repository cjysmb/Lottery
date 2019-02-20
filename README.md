# Lottery

Ethereum and Hyperledger design Pattern

How to View it

First, Open Draw.io on web browser

Second, Drag the file.

# For Ethereum Design Folder

- SimpleLottery_Eth.xml

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

# For Hyperledger Design Folder

- SimpleLottery_Hyper.xml

- First, User will register and run the app
- The system will Set lottery duration and save to world state
- User will buy ticket/s
- When user will bought a ticket, System will get the identity of user.
- After that, system will add the ID's of user to list and save it to world state
- When user will draw the winner.
- System Generate new hash from block hash to determine who is the winner
- Parse hash to unsigned integer to set randomize and choose the winner
- After that system will get the unsigned integer which provide a winner's info
- system will set the winner and save it to wolrd state 
- System will Get winner's ID.
- Withdraw the prize and the system will transfer to winner's address
- END


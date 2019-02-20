# Lottery

Ethereum and Hyperledger design Pattern

How to View it

First, Open Draw.io on web browser

Second, Drag the file.

# For Ethereum Design Folder

~ SimpleLottery_Eth.xml

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
_____________________________________________________________________________________________________________________________
~ recurring_lottery_eth.xml

- The user will initiate the contract
- System will provide new round
- The System will Set lottery duration and save to world state the total duration
- The user will load contract address
- The user will buy ticket
- The System will end the time or duration lapsed
- User will draw the winner
- When user draw the winner, the system will generate random unsigned integer
- After that, system will Use the generated integer to select an adress to Ticket list in world state
- After that, system will Assign winner's address that will retrieved in world state
- When the address verified successfully, the user will withdraw the prize.
- When withdrawing the prize the system will transfer balance to winner's address
- Add 1 to round counts
- The system will initiate new rounds
- If the round counts is less than or equal to 100, the system will be deleted 1 round
_____________________________________________________________________________________________________________________________

~ RNG LOttery _ ETH

- User submits commitment hash when buying a tickets
- User will choose what number they want to submit
- When user submitted their number, system will save the secret number and address to ticketlist in world state
- When ticketing period is over, user cannot purchased any tickets.
- When ticketing period is over, All user must reveal their secret number to know who is the winner
- After revealing, the system will verify whose secret number was the winner
- If the users failed to submit their numbers and addresses they will drop to Lottery.
- System will draw the winner and verify if the number is existing.
- Generate random number, it will enable to select the user’s address to ticketlist.
-Generate random seed for picking a winner, this is random seed to determine the winner. Each time a secret number is revealed, the seed is modified to incorporate the reveal.
- Balance will be added to user’s address and will added to world state to verify the address of the user.
_____________________________________________________________________________________________________________________________
# For Hyperledger Design Folder

~ SimpleLottery_Hyper.xml

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
_____________________________________________________________________________________________________________________________
~ recurring_lottery_hyperledger.xml

- First, User will register and run the app
- The system will Set lottery duration and save to world state
- System will draw a new round for lottery
- System will set a duration
- Participants buy a ticket/s
- When user will bought a ticket, System will get the identity of user.
- After that, system will add the ID's of user to list and save it to world state
- When user will draw the winner.
- System Generate new hash from block hash to determine who is the winner
- Parse hash to unsigned integer to set randomize and choose the winner
- After that system will get the unsigned integer which provide a winner's info
- system will set the winner and save it to wolrd state 
- System will Get winner's ID.
- Withdraw the prize and the system will transfer to winner's address
- When withdrawing the prize the system will transfer balance to winner's address
- Add 1 to round counts
- The system will initiate new rounds
- If the round counts is less than or equal to 100, the system will be deleted 1 round
_____________________________________________________________________________________________________________________________
RNG Lottery _ Hyperledger

- User’s must register first and run the application.
- Every buyer submits a commitment hash when they buy a ticket.
- User’s is generating their number which they want to submit.
- User’s secret number and address will be added to ID list..
- Ticketing period is over. Tickets cannot be purchased after this period.
- User’s must reveal their own secret number.  All reveals must occur after the ticket deadline and before the reveal deadline.
- Verifying of commitment hash and must match the commitment submitted with the ID.
- If failed to submit their own number and address, dropped from the lottery.
- Generate new hash from block hash, it will enable to select the user’s address to ID list.
- Generate random seed for picking a winner, this is random seed to determine the winner. Each time a secret number is revealed, the seed is modified to incorporate the reveal.
- Balance will be added to user’s ID and will added to world state to verify the address of the user.
- User’s wallet will be updated.


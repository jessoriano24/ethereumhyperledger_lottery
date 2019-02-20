# ethereumhyperledger_lottery
"# ethereumhyperledger_lottery" 

This repository is about the documentation and design of both ethereum and hyperledger in lottery.

To view the design:
1. Clone or download the repository.
2. Go to draw.io
3. Open the folder and drag the file on the draw.io.

# ethereum folder
"# simple_loterry_eth.xml" 

1. Inital contract
Here, the lottery system will set the duration time of the lottery. It can be second, minutes, hours or day. Once the duration time was set, It will inserted on the world state.
2. Load contract
Once the contract loaded, the user can now buy a ticket. The user's address will add to ticket list and inserted on the world state.
3. Draw winner
To draw a winner, it will generate a random unsigned  integer and it will used to select an address to ticket list. Then it will assign winner's address. The address will be inserted on the world state.
4. Withdraw
Once the draw winner was done, the user winner can now withdraw. To withdraw, first, the system will request winners address to transfer the balance to user's address and insert it on the world state. Once it was inserted, The system can now transfer the balance on user's address. Then the user can now received the prize.

"# recurring_loterry_eth.xml" 

1. Inital contract
Here, the lottery system will set the duration time of the lottery and have a new round once the duration time is done. It can be second, minutes, hours or day. Once the duration time was set, It will inserted on the world state.
2. Load contract
Once the contract loaded, the user can now buy a ticket. The user's address will add to ticket list and inserted on the world state.
3. Draw winner
To draw a winner, it will generate a random unsigned  integer and it will used to select an address to ticket list. Then it will assign winner's address. The address will be inserted on the world state.
4. Withdraw
Once the draw winner was done, the user winner can now withdraw. To withdraw, first, the system will request winners address to transfer the balance to user's address and insert it on the world state. Once it was inserted, The system can now transfer the balance on user's address. Then the user can now received the prize. If the round reached 100, round can be deleted (optional).

"# rng_loterry_eth.xml" 
1. Buy ticket
Here, once the user bought ticket, it will submit the commitment hash and generate address and secret number. The user's address will be added and secret number to the ticket list. The system will set the duration time for lottery and ticket deadline the inserted the address on the world state.
2. Reveal address and secret number
The system will verify the commitment hash and adding it to the address of sender. If failed to reveal and submit the address and secret number, it will dropped from the lottery.
3. Draw winner
To draw a winner, it will generate a random unsigned  integer and it will used to select an address to ticket list. Then it will assign winner's address. The address will be inserted on the world state.
4. Withdraw
Once the draw winner was done, the user winner can now withdraw. To withdraw, first, the system will request winners address to transfer the balance to user's address and insert it on the world state. Once it was inserted, The system can now transfer the balance on user's address. Then the user can now received the prize.

"# powerball_loterry_eth.xml" 
1. Inital contract
Here, the lottery system will set the duration time of the lottery and have a new round once the duration time is done. It can be second, minutes, hours or day. Once the duration time was set, It will inserted on the world state.
2. Load contract
Once the contract loaded, the user can now buy a ticket. The user will enter 6 digits. The limit number is 1-69. The user's address will add to ticket list and inserted on the world state.
3. Draw winner
To draw a winner, it will generate a random unsigned  number and it will used to select an address to ticket list. It will check the user's number, Then it will assign winner's address. The address will be inserted on the world state.
4. Withdraw
Once the draw winner was done, the user winner can now claim. To claim, first, the system will request winners address to transfer the balance to user's address and insert it on the world state. Once it was inserted, The system can now transfer the balance on user's address. Then the user can now received the prize.

# hyperledger folder
"# simple_loterry_hyperledger.xml" 




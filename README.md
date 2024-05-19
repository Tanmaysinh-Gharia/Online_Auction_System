# Online Auction System

## Overview
This Java program implements a simple online auction system, allowing users to create auctions, add bidders, and manage bids. The main functionalities include:

- Creating auctions and assigning lots
- Adding bidders
- Opening auctions for bidding
- Retrieving the current bid on a lot
- Placing bids
- Closing auctions
- Reporting winning bids for all lots in an auction

## File Structure
- `OnlineAuctionSystem.java`: The main Java file containing the implementation of the auction system.
- `README.md`: This readme file.

## How to Run
1. **Compile the Program:**
   Open a terminal and navigate to the directory containing `OnlineAuctionSystem.java`. Compile the program using:
   ```sh
   javac OnlineAuctionSystem.java
   ```

2. **Run the Program:**
   After compilation, run the program using:
   ```sh
   java OnlineAuctionSystem
   ```

## Functionalities
### Main Menu
When you run the program, you will be presented with a menu of options:
1. Create Auction and Assign Lots
2. Add Bidder
3. Open an Auction for Bidding
4. Retrieve the Current Bid on a Lot
5. Automatic Bid Incriment 
6. Close an Auction
7. Report on the Winning Bids for All Lots in an Auction

### Create Auction and Assign Lots
- Enter an auction name.
- Assign lots by entering lot numbers, bid starting amounts, and minimum bid increments.
- End lot insertion by entering `-1`.

### Add Bidder
- Enter the name of the bidder.
- The system will assign a unique ID to the bidder.

### Open an Auction for Bidding
- Enter the auction ID to start.
- Provide the file path to dispatch data from it (file should contain bid data).

### Retrieve the Current Bid on a Lot
- We can retrive the current Bid on a lot by lot number.

### Automatic Bid Increment 
- If user provides bid more than minimum bid amount then system bids from the users side with the difference of minimum bid difference and closes at amount of bid given.

### Close an Auction
- Assignment of Lots to users.

### Report on the Winning Bids for All Lots in an Auction
- Which user won how many bids on which price and all details.

## Code Structure
### Main Class: `OnlineAuctionSystem`
- **Static Variables:**
  - `bid_ID`: Counter for bidder IDs.
  - `auct_ID`: Counter for auction IDs.
  - `auctioMap`: HashMap storing auction details.
  - `biddMap`: HashMap storing bidder details.

- **Methods:**
  - `Create_Auction(String Auc_name, int lot, int min_bid, int min_bid_Incrm)`: Creates an auction with specified parameters.
  - `create_Bidder(String Bidr_name)`: Creates a bidder with the specified name.
  - `load_bids(String file_name)`: Loads bids from a specified file.
  - `main(String[] args)`: The main method handling user input and interaction.

### Future Enhancements
- Implement functionalities to retrieve the current bid on a lot.
- Implement the functionality to place a bid on a lot.
- Implement closing of an auction and reporting winning bids.

## Usage Example
Here is an example of how to use the system:

1. Create an Auction:
   - Choose option 1.
   - Enter "Auction1" as the auction name.
   - Add lots and their details.
   - End lot insertion with `-1`.

2. Add a Bidder:
   - Choose option 2.
   - Enter "Bidder1" as the bidder's name.

3. Open an Auction for Bidding:
   - Choose option 3.
   - Enter the auction ID (e.g., 0).
   - Provide the file path containing bid data.

This will allow you to start an auction and add bidders. The system is currently a work in progress, and additional functionalities can be implemented as needed.

## Error Handling
- The program includes basic error handling for invalid inputs and empty files.
- Future versions should include more robust error handling and validation.

## Dependencies
- Java Standard Library

## Contact
For any issues or enhancements, please contact the developer at [tanm280604@gmail.com].

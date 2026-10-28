# AUCTION-Items
ITs presented byt he group 6

AUCTION SYSTEM — Project Idea / Plot
Project Title: Auction System Using AVL Tree (Self-Balancing Binary Search Tree)
Project Idea
The Auction System is a C++ program that allows users to participate in online-style auctions. Users can register their names and receive an automatically generated four-digit ID number. After logging in, they can browse available auction items, view item details and pictures, post their own items for auction, and place bids on items they want to purchase.

Each item has a starting bid, and users can submit higher bids to compete with other bidders. The system automatically tracks the current highest bid and displays the bidder's name and ID. When the auction ends, the user with the highest valid bid is declared the winner.

The system uses an AVL Tree, a self-balancing Binary Search Tree, to organize auction item records and support efficient searching and insertion. The tree maintains a balanced structure through rotations, allowing these operations to run in \(O(\log n)\) time.
Project Plot
The system begins when a user opens the Auction System and chooses to register or log in. After successfully entering the system, the user's name and ID number are displayed at the top of the menu.

The user can then browse the available auction items, view their names, pictures, starting bids, and current highest bids. If the user wants to sell an item, they can post it for auction by providing its name, description, picture, and starting bid.

When a user selects an item, the system displays its details and allows the user to place a bid. The system checks whether the new bid is higher than the current highest bid. If it is valid, the system updates the highest bid and records the bidder's information. If the bid is too low, the system rejects it and asks the user to enter a higher amount.

After placing a bid, the user can choose to browse other items or stop bidding. When the auction closes, the system identifies the highest valid bidder as the winner and displays the winning amount, item name, winner's name, and ID number.

Throughout the process, the AVL Tree helps manage the auction item records efficiently, making the system organized and easier to search.
Main Objectives
1. To develop a C++ auction system with user registration and automatically generated ID numbers.
2. To allow users to post, browse, and select auction items.
3. To implement a bidding system that tracks and updates the highest bid.
4. To automatically identify the winner based on the highest valid bid when the auction closes.
5. To apply AVL Tree operations for efficient item searching and insertion.
6. To provide a simple and user-friendly console interface for auction participants.

Expected Output
The finished program should allow users to register, browse and post items, place bids, view current highest bids, and determine auction winners. It will demonstrate how an AVL Tree can be applied to a practical auction management system while maintaining efficient data organization and retrieval.

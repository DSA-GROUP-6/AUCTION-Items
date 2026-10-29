# Project Title: Auction System Using AVL Tree (Self-Balancing Binary Search Tree)
ITs presented by the group 6

The project is an interactive Online Auction System designed to allow users to securely log in, browse active auction items, post new listings with starting bid prices, and place competitive bids in real time.   

To handle high-volume bidding without system slowdowns, the backend utilizes an AVL Tree (Self-Balancing Binary Search Tree). This data structure ensures that inserting new bids and identifying the current highest bidder always operates at maximum efficiency (O(\log n)O(logn) performance).   

The operational flow of the system follows a logical sequence from start to finish, as illustrated in the system flowchart:   

Phase 1: User Entry & Main Menu Navigation
1. System Initialization: The user launches the application and is presented with the Main Menu Hub (2B).
     
2. Action Selection: The system prompts the user to select one of three primary paths:   
  •	Browse Auction Items   
  •	Post Item for Auction   
  •	View Highest Bid   

Phase 2: Posting a New Item for Auction
1. Initiation: The user selects "Post Item for Auction" from the main menu.   
2  Data Input: The system requests inputs for:
   
  •	Item details/name   
  •	Starting bid amount   


3. Display & Confirmation: The system outputs the newly created listing showing the item name and starting bid, then prompts: "Save?"   
4. Data Storage:
  •	If YES: The item is saved directly into the main database (4D), making it immediately available for bidding. The system then loops back to the main menu (3C).   
  •	If NO: The item is discarded, and the session terminates (5E).  
Phase 3: Browsing Items & Placing Bids (AVL Tree Execution)
1. Item Retrieval: The user selects "Browse Auction Items". The system queries the database (4D) to check if any items are stored:   
  •	If NO items exist: The user is redirected back to the main menu (3C). 
  •	If items exist: The available auction items are displayed on screen.   

2. Item & Bid Selection: The user selects a specific item and enters their proposed Bid Amount.   
3. AVL Tree Processing: The system executes the AVL Tree Method to record and evaluate the new bid:    
  •	The bid is inserted into the AVL tree structure.   
  •	Dynamic rotations automatically balance the tree, evaluating node values to immediately determine and track the leading bid.    
4. Loop Option: The system asks: "Bid Again?"   
  •	If YES: The user returns to the main menu loop (3C).   
  •	If NO: The session exits (5E).   

Phase 4: Viewing the Highest Bid
1. Query Request: The user selects "View Highest Bid" from the main menu.   
2. Instant Retrieval: The system traverses the balanced AVL Tree root node to extract and display the current winning bidder and bid amount instantly.   
3. Return to Hub: After displaying the highest bidder, the system returns the user directly to the main menu (3C).


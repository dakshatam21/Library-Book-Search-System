# Library-Book-Search-System

The Library Book Search System is a fast and user-friendly web app that allows users to search books with real-time suggestions. It uses a Trie for quick prefix-based searching and a Hash Table/database lookup for instant exact results, making the search process efficient and smooth even with large data.


Features
Search by Book ID, Title, or Author
O(1) average time complexity using Hash Table lookup
Trie-based autocomplete with real-time suggestions
MySQL database backend
Simple and clean HTML/CSS user interface
Displays search time for analysis


Technologies Used
Frontend: HTML, CSS, JavaScript
Backend: Node.js, Express.js
Database: MySQL
Data Structures: Hash Table, Trie


Project Structure
/Library_Search
│── library.html      → Frontend UI
│── library.css       → Styling
│── library.js        → Frontend logic + Trie suggestions
│── server.js         → Backend + Trie implementation
│── library.sql       → Database schema and sample book records


Setup Instructions

1. Install Dependencies
npm install express mysql cors

2. Import Database
Run this inside MySQL:
SOURCE library.sql;

3. Start the Server
node server.js

4. Open the Application
Open library.html in your browser.


How It Works ?

When the user types in the search bar, the Trie provides live suggestions based on title or author prefixes.
When the user clicks “Search”, the backend performs a Hash Table + SQL lookup to get the exact match.
The result and search time are displayed instantly.


Why Hash Table + Trie?
Hash Table: Provides fast O(1) lookup for exact book search.
Trie: Provides smart, fast suggestions even with partial or incomplete input.
Using both makes the system efficient, accurate, and user-friendly.


Future Enhancements
Add admin panel to insert or update books
Add user authentication or login
Add fuzzy search (auto-correct spellings)


Author
Dakshata Mhatre

🏏 Player Management System
<p align="center"> <img src="https://img.shields.io/badge/Language-C-blue?style=for-the-badge&logo=c" alt="C"> <img src="https://img.shields.io/badge/Project-Mini%20Project-orange?style=for-the-badge" alt="Mini Project"> <img src="https://img.shields.io/badge/Status-Completed-success?style=for-the-badge" alt="Status"> </p> <p align="center"> <b>A simple and efficient console-based Player Management System built using C programming.</b> </p>
📌 About The Project
Player Management System is a console-based mini project developed in C programming to manage and maintain cricket player records.
The project provides a simple menu-driven interface that allows users to add, view, search, update, delete, and analyze player information.

This project was created to practice and demonstrate important C programming concepts such as:

Structures
Pointers
Functions
Arrays
Strings
Dynamic Memory Allocation
Searching
Sorting
CRUD Operations
Menu-driven programming
🎯 Project Objectives
The main objectives of this project are:
📋 Store player information efficiently.
🔍 Search for players using different criteria.
✏️ Update existing player records.
🗑️ Delete player records.
📊 Analyze player performance.
🏆 Display top-performing players.
🧠 Improve understanding of structures and pointers in C.
💾 Practice dynamic memory allocation.
⚡ Features
👤 Player Management
The system stores the following information for each player:
Field	Description
👤 Player Name	Name of the player
🔢 Jersey Number	Unique jersey number
🏟️ Matches Played	Total matches played
🏏 Runs	Total runs scored
🎯 Wickets	Total wickets taken

➕ Create Player Records
Users can enter details of multiple players through the console.
Example:

Enter Player Name: Virat
Enter Jersey Number: 18
Enter Matches Played: 250
Enter Runs: 12898
Enter Wickets: 4

📋 Display Players
Displays all currently stored player records in the database.
Example:

Name       : Virat
Jersey No. : 18
Matches    : 250
Runs       : 12898
Wickets    : 4

🔍 Search Player
Players can be searched using:
1. Jersey Number
2. Player Name

This makes it easy to find a specific player from the database.
✏️ Update Player
Existing player information can be modified.
The following fields can be updated:

Player Name
Jersey Number
Matches Played
Runs
Wickets
🗑️ Delete Player
Players can be removed from the database using:
Jersey Number
Player Name
After deletion, the remaining records are shifted to maintain the array structure.
🏆 Top 3 Players
The project provides player performance analysis based on:
🏏 Top 3 Players with Most Runs
🎯 Top 3 Players with Most Wickets
📉 Top 3 Players with Least Runs
📉 Top 3 Players with Least Wickets

The program uses sorting techniques to arrange players according to their performance.
🖥️ Menu
The application provides a simple menu-driven interface:
========================================
       PLAYER MANAGEMENT SYSTEM
========================================

1. Create
2. Display
3. Search
4. Update
5. Delete
6. Show Top 3 Players
7. Exit

Enter your choice:

🧠 Concepts Used
This project demonstrates several important C programming concepts.
🔹 Structure
A struct is used to store all information related to a player.
typedef struct player
{
    char player_name[20];
    int jersey_num;
    int match_played;
    int runs;
    int wicket;
} player;

🔹 Pointers
Pointers are used to pass the player array to functions and modify the original data.
void display(player *p, int size);

🔹 Dynamic Memory Allocation
Memory for player records can be allocated dynamically using:
player *p = malloc(arr_size * sizeof(player));

🔹 Strings
The project uses functions such as:
strcmp()
strcpy()

for player-name searching and copying.
🔹 Searching
Linear searching is used to locate players based on their:
Name
Jersey Number
🔹 Sorting
Sorting is used to determine the top and bottom performers based on:
Runs
Wickets
🔹 CRUD Operations
The project implements the basic database operations:
Operation	Function
➕ Create	Add player records
📖 Read	Display/search records
✏️ Update	Modify records
🗑️ Delete	Remove records

🛠️ Technologies Used
<p> <img src="https://img.shields.io/badge/C-Programming-blue?style=flat-square&logo=c" alt="C"> <img src="https://img.shields.io/badge/GCC-Compiler-red?style=flat-square" alt="GCC"> <img src="https://img.shields.io/badge/Git-Version%20Control-orange?style=flat-square&logo=git" alt="Git"> <img src="https://img.shields.io/badge/GitHub-Repository-black?style=flat-square&logo=github" alt="GitHub"> </p>
Programming Language: C
Compiler: GCC
IDE: Any C-compatible IDE
Version Control: Git
Repository: GitHub
📂 Project Structure
Player-Management-System/
│
├── player_management.c
├── README.md
└── LICENSE

🚀 Getting Started
1️⃣ Clone the Repository
git clone https://github.com/your-username/Player-Management-System.git

2️⃣ Navigate to the Project
cd Player-Management-System

3️⃣ Compile the Program
Using GCC:
gcc player_management.c -o player_management

4️⃣ Run the Program
Linux / macOS:
./player_management

Windows:
player_management.exe

🧪 Sample Player Data
The following data can be used to test the application:
Player	Jersey	Matches	Runs	Wickets
🏏 Virat	18	250	12898	4
🏏 Rohit	45	243	10500	9
🎯 Bumrah	93	150	350	310
⭐ Jadeja	8	200	3200	280
🧤 Pant	17	120	4200	5

📸 Sample Output
========================================
       PLAYER MANAGEMENT SYSTEM
========================================

1. Create
2. Display
3. Search
4. Update
5. Delete
6. Show Top 3 Players
7. Exit

Enter your choice: 2


-------- PLAYER DETAILS --------

Player 1
Name       : Virat
Jersey No. : 18
Matches    : 250
Runs       : 12898
Wickets    : 4

Player 2
Name       : Rohit
Jersey No. : 45
Matches    : 243
Runs       : 10500
Wickets    : 9

--------------------------------

📊 Top 3 Example
For the sample data, the program can produce results such as:
🏏 Most Runs
1. Virat   - 12898 runs
2. Rohit   - 10500 runs
3. Pant    - 4200 runs

🎯 Most Wickets
1. Bumrah  - 310 wickets
2. Jadeja  - 280 wickets
3. Rohit   - 9 wickets

🔄 Program Flow
              ┌─────────────────────┐
              │       START         │
              └──────────┬──────────┘
                         │
                         ▼
              ┌─────────────────────┐
              │ Allocate Memory     │
              └──────────┬──────────┘
                         │
                         ▼
              ┌─────────────────────┐
              │    Display Menu     │
              └──────────┬──────────┘
                         │
          ┌──────────────┼──────────────┐
          │              │              │
          ▼              ▼              ▼
       Create         Display        Search
          │              │              │
          └──────────────┼──────────────┘
                         │
              ┌──────────▼──────────┐
              │ Update / Delete     │
              └──────────┬──────────┘
                         │
                         ▼
              ┌─────────────────────┐
              │     Top 3 Stats     │
              └──────────┬──────────┘
                         │
                         ▼
                  ┌────────────┐
                  │    Exit    │
                  └────────────┘

🔮 Future Improvements
The current project is focused on practicing core C concepts. It can be extended with:
💾 File handling for permanent data storage
🔐 User authentication
📊 Advanced player statistics
🏏 Separate batsman and bowler categories
🔎 Advanced filtering and searching
📈 Performance graphs
🗄️ Database integration
🖥️ Graphical User Interface
🌐 Web-based player management system
⚠️ Current Limitations
Data is stored in memory and may be lost when the program exits.
Player names are limited by the allocated character array.
The application is currently console-based.
No external database is used.
Input validation can be improved.
🎓 Learning Outcomes
After completing this project, the following concepts can be practiced:
✔ Structures
✔ Pointers
✔ Functions
✔ Arrays
✔ Strings
✔ Dynamic Memory Allocation
✔ Searching Algorithms
✔ Sorting Algorithms
✔ CRUD Operations
✔ Menu-Driven Programming
✔ Memory Management

Fork the repository.
Create a new branch.
Make your changes.
Commit your changes.
Push the branch.
Create a Pull Request.
git checkout -b feature/new-feature
git add .
git commit -m "Add new feature"
git push origin feature/new-feature


🧪 Sample Player Data
    player p[5] = 
    {
        {"Virat", 18, 250, 12898, 4},
        {"Rohit", 45, 243, 10500, 9},
        {"Bumrah", 93, 150, 350, 310},
        {"Jadeja", 8, 200, 3200, 280},
        {"Pant", 17, 120, 4200, 5}
    };

    
👨‍💻 Author 
Lokesh Pusdekar
💻 C Programming | 📚 Student | 🚀 Aspiring Devel

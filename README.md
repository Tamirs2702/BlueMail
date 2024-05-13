# TicTacToe

simple web application built with Node.js, Express, and Socket.IO for real-time communication. It allows multiple users to play a game with each other in real-time.

## Installation

1. Clone the repository to your local machine:

    ```
    git clone https://github.com/Tamirs2702/BlueMail.git
    ```

2. Navigate to the project directory:

    ```
    cd BlueMail
    ```

3. Install dependencies:

    ```
    npm install
    ```

## Usage

1. Start the server:

    ```
    node index.js
    ```

2. Access the application in your web browser at `http://localhost:3000`.

3. Interact with the application by opening multiple browser tabs or windows and navigating to `http://localhost:3000`.

## Game Structure and Flow

BlueMail is structured as a simple web-based tic-tac-toe game. The main entities used in the game are players, game boards, and game sessions. When a player connects to the server, they are assigned to a game session. Each session can have two players. Once two players are connected, the game begins.

The basic flow of the game is as follows:
- Players join the game session.
- Each player takes turns making moves on the game board.
- After each move, the server checks for a win condition.
- If a win condition is met, the game ends and the winner is declared.
- If no win condition is met, the game continues until all cells on the board are filled, resulting in a draw.

## Win Condition Check

After each move, the server checks for a win condition by examining the current state of the game board. It checks for three consecutive marks (either 'X' or 'O') in a row (horizontal, vertical, or diagonal). If a win condition is found, the game ends and the player who achieved the win condition is declared the winner.

## Dependencies

- express
- socket.io



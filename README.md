# Bulls Cows - Operating Systems Course


Bulls and Cows is a 2 player game. 
One player thinks of a number, while the other player tries to guess it.
The number to be guessed must be a 4 digit number, using only digits from 1 - 9, each digit atmost once. 
For every guess that the player makes, he gets 2 values - the number of bulls and the number of cows. 

1 bull means the guess contains and the target number have 1 digit in common, and in the correct position.
1 cow means the guess and the target have 1 digit in common, but not in correct position.

The game ends with win if one of the player guessed right the other 4 digits.
It can also ends with tie if both of the players guessed right the other 4 digits in the same turn.


# Server
Manages the game. It receives incoming communications from the client, calculates the game results, and distributes messages between clients. 
The server it waits for two clients to connects, then starts the game, with respect to all the rules mentioned above.

# Client
The client's interface of the game. The software receives commands from the player, and sends them to the server.
The software receives updates from the server, and presents them to the player. The client software does not understand the rules of the game.
It is a bridge between the players and the server software.

# Advanced Programming Conepts
Deep utilizing of thread concepts in operating systems in general and Windows in particular.

• Working with several threads in parallel.

• Use Mutex and Semaphore to synchronize access to shared resources between threads.

• Use Mutex and Semaphore to synchronize access to shared memory between threads.

Deep utilizing of computer communication.

• Using Sockets TCP:

  WSAStartup, WSACleanup 
  ,socket 
  ,bind 
  ,listen 
  ,accept 
  ,recv 
  ,connect 
  ,closesocket 
  ,send.

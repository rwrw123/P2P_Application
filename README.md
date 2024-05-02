# P2P_Application
This program enables a real-time communication between a client and server over network using socket. It's designed to handle multiple cline connections concurrently, with each client being able to send messages to the server. The serer processes those messages and perform actions based on the content recieves. 

## Features
### Real-Time Communication: 
      - Instant message passing from client to server
### JSON Message Encoding:
      - Encodes and decodes messages in JSON format for flexibility and ease of data handling
### Robust Error Handling:
      - Implements try-except blocks to manage exceptions, ensuring stable connection management

## Requirements
      Python 3.x

## Testing
      1. Run the server script:
      python server.py
      - The server will start listening for incoming connections and process messages when recieves them
      2. Run the client script:
      python client.py
      - Follow the on-screen prompts to send message to the server
<img width="512" alt="Screen Shot 2024-04-07 at 10 59 38 PM" src="https://github.com/rwrw123/P2P_Application/assets/113308286/05afddc7-aa0a-4a29-be82-092b972085a2">
<img width="534" alt="Screen Shot 2024-04-07 at 10 59 23 PM" src="https://github.com/rwrw123/P2P_Application/assets/113308286/87e516ab-42a5-48ae-ae59-cd3c9b2eb0b9">

## Database
### Users: Stores user information.
- user_id: Unique identifier for each user (INT, AUTO_INCREMENT, PRIMARY KEY).
- username: Username of the client (VARCHAR, NOT NULL).
- created_at: Timestamp when the user was created (DATETIME, DEFAULT CURRENT_TIMESTAMP).
### Messages: Stores messages sent by users.
- message_id: Unique identifier for each message (INT, AUTO_INCREMENT, PRIMARY KEY).
- user_id: Reference to the user who sent the message (INT, FOREIGN KEY REFERENCES Users(user_id)).
- content: Text content of the message (TEXT, NOT NULL).
- timestamp: Timestamp when the message was sent (DATETIME, DEFAULT CURRENT_TIMESTAMP).
### Prerequisties
- MySQL Server 5.7 or higher
### Users Table
<img width="613" alt="Screen Shot 2024-05-01 at 8 10 54 PM" src="https://github.com/rwrw123/P2P_Application/assets/113308286/402d4b36-f8fc-4712-be61-37c461f1b3bb">

### Messages Table
<img width="607" alt="Screen Shot 2024-05-01 at 8 11 49 PM" src="https://github.com/rwrw123/P2P_Application/assets/113308286/6ed8c8d4-0eb5-49e3-9613-86336b910fb8">



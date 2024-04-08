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


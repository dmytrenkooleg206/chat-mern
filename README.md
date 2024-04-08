# Connectify - Real-Time Chat Application
![image](https://github.com/ankitjangidx/Chatify/assets/100501722/103fb812-c71b-4744-9881-734cdce16370)
![image](https://github.com/ankitjangidx/Chatify/assets/100501722/f272936d-18b8-4c74-8584-18bb5227ca49)
![image](https://github.com/ankitjangidx/Chatify/assets/100501722/aa5103ed-ca77-4113-ac8c-21f027e12e29)




## Project Description

Connectify is a cutting-edge real-time chat application designed to revolutionize communication among users. With its modern interface and robust features, Connectify offers a seamless and immersive chat experience like never before. Built on the powerful MERN (MongoDB, Express.js, React.js, Node.js) stack and integrated with WebSocket technology, Connectify brings instant messaging to the next level.

Connectify aims to redefine communication by providing:
- **Real-Time Messaging:** Say goodbye to delays with Connectify's WebSocket integration, enabling lightning-fast message delivery and updates.
- **Intuitive User Interface:** Navigate effortlessly through Connectify's sleek and user-friendly interface, designed for maximum convenience and engagement.
- **Secure Authentication:** Rest assured knowing your data is safe with Connectify's secure JWT-based authentication system, ensuring only authorized users access the platform.
- **Scalable Architecture:** Built on a scalable architecture, Connectify can effortlessly handle growing user bases without compromising performance.


## Front End

Powered by React.js, Connectify's front end offers a seamless and responsive user experience. Key features include:
- **Real-Time Chat Interface:** Engage in fluid conversations with Connectify's intuitive chat interface, ensuring smooth communication among users.
- **Dynamic User Authentication:** Seamlessly log in and register with Connectify's dynamic authentication system, providing secure access to the platform's features.
- **Interactive Chat Rooms:** Create and manage individual and group chat rooms effortlessly, fostering collaboration and connection among users.
- **Instant Notifications:** Stay updated with real-time notifications for incoming messages and other pertinent events, ensuring users never miss a beat.

## Back End

Connectify's back end, powered by Node.js and Express.js, offers robust server-side functionality. Key features include:
- **RESTful APIs:** Access Connectify's features seamlessly with its RESTful API endpoints, enabling smooth communication between the front end and back end.
- **WebSocket Integration:** Harness the power of WebSocket technology with Connectify's real-time communication capabilities, ensuring instant message delivery and updates.
- **MongoDB Integration:** Interact seamlessly with MongoDB, Connectify's primary database, ensuring efficient storage and retrieval of user data, chat messages, and application information.
- **Secure Authentication:** Authenticate users securely with JWT-based authentication, providing a safe and reliable access mechanism to the platform's resources.



## API Design

Connectify's API adheres to RESTful principles, offering endpoints for various functionalities such as user authentication, chat room creation, message sending, and user management. Sample API endpoints and their functionalities include:


### Chat Routes

#### Access Chat
- **Method:** POST
- **Endpoint:** `/api/chat`
- **Middleware:** protect
- **Controller:** accessChat
- **Description:** Allows users to access a chat room.

#### Fetch Chats
- **Method:** GET
- **Endpoint:** `/api/chat`
- **Middleware:** protect
- **Controller:** fetchChats
- **Description:** Retrieves all existing chat rooms.

#### Create Group Chat
- **Method:** POST
- **Endpoint:** `/api/chat/group`
- **Middleware:** protect
- **Controller:** createGroupChat
- **Description:** Creates a new group chat.

#### Rename Group
- **Method:** PUT
- **Endpoint:** `/api/chat/rename`
- **Middleware:** protect
- **Controller:** renameGroup
- **Description:** Renames an existing group chat.

#### Remove From Group
- **Method:** PUT
- **Endpoint:** `/api/chat/groupremove`
- **Middleware:** protect
- **Controller:** removeFromGroup
- **Description:** Removes a user from a group chat.

#### Add To Group
- **Method:** PUT
- **Endpoint:** `/api/chat/groupadd`
- **Middleware:** protect
- **Controller:** addToGroup
- **Description:** Adds a user to a group chat.

### Message Routes

#### Get All Messages
- **Method:** GET
- **Endpoint:** `/api/message/:chatId`
- **Middleware:** protect
- **Controller:** allMessages
- **Description:** Retrieves all messages from a specific chat room.

#### Send Message
- **Method:** POST
- **Endpoint:** `/api/message`
- **Middleware:** protect
- **Controller:** sendMessage
- **Description:** Sends a message to a specific chat room.

### User Routes

#### Get All Users
- **Method:** GET
- **Endpoint:** `/api/user`
- **Middleware:** protect
- **Controller:** allUsers
- **Description:** Retrieves all users.

#### Register User
- **Method:** POST
- **Endpoint:** `/api/user`
- **Controller:** registerUser
- **Description:** Registers a new user.

#### Authenticate User
- **Method:** POST
- **Endpoint:** `/api/user/login`
- **Controller:** authUser
- **Description:** Authenticates user credentials and generates a JWT token.


## Future Enhancements

Connectify has a roadmap for future enhancements, including:
- Implementing end-to-end encryption for secure message transmission.
- Adding multimedia support for sharing images, videos, and files.
- Enhancing user experience with additional features such as emojis, reactions, and chatbots.
- Improving scalability and performance through optimized database queries and caching mechanisms.

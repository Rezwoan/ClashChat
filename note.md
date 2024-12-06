# Clash of Clans Platform - Clan Stats and Chat

## Features

### **Account Claiming**

-   [ ] Player can provide **CoC API Key** to claim account.
-   [ ] Platform verifies API key and retrieves player details from CoC API.
-   [ ] Link player's CoC account to platform profile after successful verification.
-   [ ] Grant access to **private chat** and **public chat** once account is linked.

### **Chat System**

-   [ ] Implement **Public Chat** for open communication.
-   [ ] Implement **Private Chat** for messaging within the same clan or friends.
-   [ ] Apply message filtering (anti-spam, inappropriate content) for both chat types.

## Data to be Pulled from CoC API

### **Clan Stats:**

-   [ ] Pull **Clan Name**.
-   [ ] Pull **Clan Tag**.
-   [ ] Pull **Clan Level**.
-   [ ] Pull **Clan Points**.
-   [ ] Pull **Clan Description**.
-   [ ] Pull **Clan Location (Region)**.
-   [ ] Pull **Clan Type** (War Clan, Casual, etc.).
-   [ ] Pull **War Stars**.
-   [ ] Pull **Clan Wins / Losses**.
-   [ ] Pull **Clan Members Count**.
-   [ ] Pull **Clan Leader**.
-   [ ] Pull **Clan Co-Leaders**.

### **Player Stats (for each clan member):**

-   [ ] Pull **Player Name**.
-   [ ] Pull **Player Tag**.
-   [ ] Pull **Player Level**.
-   [ ] Pull **Player Troops**.
-   [ ] Pull **Player Heroes** (Barbarian King, Archer Queen, Grand Warden, etc.).
-   [ ] Pull **Player Clan Role** (Leader, Co-Leader, Member).
-   [ ] Pull **Player Donated Troops**.
-   [ ] Pull **Player Received Troops**.
-   [ ] Pull **Player Trophies**.
-   [ ] Pull **Player War Stars**.
-   [ ] Pull **Player Battles Won / Lost**.
-   [ ] Pull **Player Clan Rank**.
-   [ ] Pull **Player Donations History**.

## Chat Types:

### **Public Chat:**

-   [ ] Implement Public Chat system for all members.
-   [ ] Ensure proper moderation and message filtering.

### **Private Chat:**

-   [ ] Implement Private Chat for messaging within the same clan or friends.
-   [ ] Ensure messages are only accessible to sender and recipient.

## Backend Implementation (Python)

### **Steps for Account Claiming:**

-   [ ] Player inputs **CoC API Key** on the platform.
-   [ ] Use API key to verify the player's account via the CoC API.
-   [ ] Link player's CoC account to platform profile.
-   [ ] Grant chat access after account verification.

### **Chat Storage and Management:**

-   [ ] Implement real-time messaging using **WebSockets** or **REST APIs**.
-   [ ] Set up **Users Table** to store player data and CoC account details.
-   [ ] Set up **Messages Table** to store message content and metadata.
-   [ ] Set up **Chats Table** to manage public/private chat groups.

### **Security:**

-   [ ] Store API keys securely.
-   [ ] Use **JWT (JSON Web Tokens)** or **OAuth2** for authentication.
-   [ ] Sanitize all inputs to prevent XSS and SQL injection attacks.

## Frontend Implementation (Vue.js)

### **Why Vue.js?**

-   [ ] Set up **Vue.js** for frontend development (single-page app).
-   [ ] Use **Vuex** for state management (store player data, chat messages, etc.).
-   [ ] Use **Vue Router** for navigation (manage different views like Home, Chat, Profile).
-   [ ] Create dynamic **Vue Components** for chat, user profile, etc.

### **Steps for Vue.js Integration:**

-   [ ] Create Vue components for **Public Chat**, **Private Chat**, and **Player Profile**.
-   [ ] Use **Vuex** for managing state (user details, chat data).
-   [ ] Implement real-time chat with **WebSockets** or **REST APIs**.
-   [ ] Integrate **Axios** or **Fetch** for making requests to the backend (account claiming, fetching stats).
-   [ ] Set up routing with **Vue Router** to handle different pages.
-   [ ] Implement authentication flow using **JWT tokens** or **OAuth2**.

## Things to Look Up on the Internet

### **Python (Backend)**

-   [ ] **Django Rest Framework (DRF)**: [DRF Documentation](https://www.django-rest-framework.org/)
-   [ ] **Flask-SocketIO**: [Flask-SocketIO Documentation](https://flask-socketio.readthedocs.io/)
-   [ ] **Django Channels**: [Django Channels Documentation](https://channels.readthedocs.io/)
-   [ ] **JWT Authentication**: [JWT Authentication with Django Rest Framework](https://simpleisbetterthancomplex.com/tutorials/real-world-django/part-10-jwt-authentication/)

### **Vue.js (Frontend)**

-   [ ] **Vue.js Documentation**: [Vue.js Official Docs](https://vuejs.org/)
-   [ ] **Vuex Documentation**: [Vuex Documentation](https://vuex.vuejs.org/)
-   [ ] **Vue Router Documentation**: [Vue Router Docs](https://router.vuejs.org/)
-   [ ] **Axios for HTTP Requests**: [Axios Documentation](https://axios-http.com/)
-   [ ] **Vue WebSockets**: [Vue WebSockets Integration Example](https://vuejs.org/v2/cookbook/websocket.html)

### **General Tools**

-   [ ] **CoC API**: [Clash of Clans API Documentation](https://developer.clashofclans.com/)

---

### References:

-   [Clash of Clans API Documentation](https://developer.clashofclans.com/)

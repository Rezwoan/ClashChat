# ClashChat

**ClashChat** is a platform designed for **Clash of Clans** players to manage their clan stats, claim their accounts via the CoC API, and engage in real-time chat with other players. Players can chat privately with clan members or participate in public discussions, all while keeping track of their player and clan statistics.

---

## Features

-   **Account Claiming**: Players can link their **Clash of Clans** account by providing their **API Key**.
-   **Clan Stats**: View detailed information about your clan, including war stats, members, and more.
-   **Player Stats**: Track player performance, including trophies, war stars, and donations.
-   **Real-time Chat**:
    -   **Public Chat**: Participate in an open chat room with your clan or all platform users.
    -   **Private Chat**: Send private messages to your clan members or friends.
-   **User Authentication**: Secure login via **Clash of Clans API** for account verification.

---

## Technologies

-   **Frontend**:
    -   **Vue.js** for building dynamic user interfaces.
    -   **Vuex** for state management and **Vue Router** for routing.
    -   **Axios** for HTTP requests to interact with the Python backend.
-   **Backend**:

    -   **Python** with **Django Rest Framework (DRF)** or **Flask** for API endpoints.
    -   **WebSockets** for real-time chat (using **Django Channels** or **Flask-SocketIO**).
    -   **JWT Authentication** for secure user sessions.

-   **Database**:
    -   Use a database (such as **PostgreSQL** or **SQLite**) for storing user, message, and clan data.

# Saby

## Overview

Saby is an open-source chatbot built using the Rasa framework. It is designed to allow users to create and manage their own services, perform financial transactions, access lifestyle information, and manage e-commerce operations. The bot also provides intelligent and humorous interactions using GPT-4 and predefined responses. The architecture is built using microservices, with MongoDB as the preferred database and Docker for containerization.

## Features

### 1. **User Authentication and Role Management**
   - **JWT-based Authentication**: Secure user login and session management.
   - **Role-Based Access Control**: Predefined roles including Customer, Service Provider, Admin, and Super Admin.
   - **Additional Security**: Features like forgot password and two-factor authentication (2FA).

### 2. **Financial Transactions**
   - **Multiple Payment Gateways**: Integration with Paystack, Flutterwave, and a custom payment API.
   - **Wallet Management**: Users can load wallets, view transaction history, and perform money transfers.
   - **Bill Payments**: Capability to pay bills directly through Saby.

### 3. **Lifestyle Information**
   - **APIs Integration**: Fetch and display information such as weather, news, exchange rates, reminders, sports scores, public holidays, health tips, stock prices, horoscope, and traffic updates.
   - **Reminders and Alerts**: Users can set and receive personalized reminders and alerts.

### 4. **E-Commerce Functionality**
   - **Platform Integration**: Connect with existing platforms like Shopify or WooCommerce.
   - **Custom Order Management**: Features for ordering food, groceries, etc., with real-time tracking, notifications, and customer reviews.

### 5. **Intelligence and Humor**
   - **GPT-4 Integration**: Handles complex queries, generates jokes, and provides intelligent responses.
   - **Predefined Responses**: Includes a set of predefined responses for jokes, trivia, and general entertainment.

## Architecture

The project is designed with a microservices architecture to ensure modularity and scalability. The main components include:

- **Rasa Bot**: Handles natural language understanding (NLU) and dialogue management.
- **Custom Actions Server**: Manages custom logic, such as service registration, order processing, and financial transactions.
- **MongoDB**: Stores user data, service details, and transaction records.
- **Docker**: Containerizes all services for easy deployment and scaling.
- **GitHub**: Used for version control and continuous integration.

## Setup and Installation

### Prerequisites

- Docker
- Docker Compose
- Python 3.8 or later

### Installation Steps

1. **Clone the Repository**:
   ```
   git clone https://github.com/yourusername/saby.git
   cd saby````

2. **Set Up Docker:**

Ensure Docker and Docker Compose are installed on your system.
Start the services using Docker Compose:

```
docker-compose up -d
```

3.** Initialize the Rasa Project:**
```
rasa init
```

4. **To start  Saby:**
```
saby run --enable-api --cors "*"
```

5.** To start the action server:**
```
saby run actions
```

# Contribution
We welcome contributions to enhance the features and functionalities of Saby. Please follow these steps to contribute:

Fork the repository.
Create a new branch for your feature (git checkout -b feature-branch).
Commit your changes (git commit -m 'Add some feature').
Push to the branch (git push origin feature-branch).
Open a pull request.

## License
This project is licensed under the MIT License - see the LICENSE file for details.

## Contact
For any questions or support, please open an issue on GitHub or contact the project maintainers at contributions@saby.ai 
   

@@ -1,2 +1,93 @@


# Crowd Campaign DApp

## Overview

The Crowd funding Campaign DApp is a decentralized application built on the Secret Network that allows anyne create a project and seek crowd funding effort from anyone. This DApp ensures people can see project and decide which one to support.

## Features

- **Create Project**: Create and Submit Detail description of your project and the amount you need to accomplish the project .
- **Project base Category**: Provide List of funding Campaign base on categories.
- **Open Project**: Provide List of funding Campaign that are open to support.
- **Support Project**: Support a campaign for a particular project.
- **Admin Dashboard**: Campus administrators can view Campaign and their various stages .
- **Voting Mechanism**: Users can upvote Campaign.

## Technologies Used

- **Secret Network**: For building private smart contracts and ensuring data privacy.
- **CosmWasm**: For writing smart contracts.
- **SecretJS**: For interacting with the Secret Network from the frontend.
- **React.js**: For building the frontend interface.
- **Node.js**: For backend server operations.

## Installation

### Prerequisites

- Node.js
- npm (Node Package Manager)
- Docker (optional, for local Secret Network setup)

### Clone the Repository

```bash
git clone https://github.com/mmanueljoe/anonymous-feedback-dapp.git
cd anonymous-feedback-dapp
```

### Install Dependencies

```bash
npm install
```

### Setup Environment Variables

Create a `.env` file in the root directory and add the following environment variables:

```
REACT_APP_SECRET_RPC_URL=https://api.scrt.network
REACT_APP_SECRET_CHAIN_ID=secret-2
REACT_APP_BACKEND_URL=http://localhost:5000
```

### Run the Application

#### Backend

Navigate to the `backend` directory and start the server:

```bash
cd backend
npm install
npm start
```

#### Frontend

Navigate back to the root directory and start the frontend:

```bash
npm start
```

### Access the Application

Open your browser and navigate to `http://localhost:3000` to use the application.

## Usage

1. **Submit Feedback**: Select a category, enter your feedback, and submit anonymously.
2. **View Feedback**: Administrators can log in to view all submitted feedback.
3. **Vote on Feedback**: Users can upvote feedback entries to highlight important issues.

## Development

### Setting Up Local Secret Network (Optional)

To set up a local Secret Network for testing, use Docker:

```bash
docker run -d -p 26657:26657 -p 1317:1317 -p 9090:9090 --name secretdev enigmampc/secret-network-sw-dev
```

This will allow you to interact with a local instance of the Secret Network.

### Running Tests

To run tests, navigate to the smart contract and frontend directories and execute the test commands:

```bash
# Smart Contract Tests
cd contracts
cargo test

# Frontend Tests
cd ../frontend
npm test
```

## Contributing

We welcome contributions to improve this project! Please fork the repository, create a new branch, and submit a pull request.

This README provides a comprehensive guide to setting up, using, and contributing to the Anonymous Feedback DApp. Feel free to customize it based on your specific setup and requirements.

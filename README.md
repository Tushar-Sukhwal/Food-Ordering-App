# MERN Stack Project with TypeScript

Welcome to our MERN (MongoDB, Express.js, React.js, Node.js) stack project template with TypeScript! This README will guide you through setting up both the backend and frontend components of the project.

## Prerequisites

Before starting, ensure you have the following installed:

- Node.js and npm (Node Package Manager)
- MongoDB
- Git (optional, but recommended)

## Backend Setup

1. Clone this repository to your local machine:

    ```bash
    git clone <repository_url>
    ```

2. Navigate to the backend directory:

    ```bash
    cd backend
    ```

3. Install backend dependencies:

    ```bash
    npm install
    ```

4. Create a `.env` file based on `.env.example` and fill in the required environment variables:

    ```plaintext
    # MongoDB Connection String
    MONGODB_CONNECTION_STRING=<your_mongodb_connection_string>

    # Auth0
    AUTH0_AUDIENCE=<your_auth0_audience>
    AUTH0_ISSUER_BASE_URL=<your_auth0_issuer_base_url>

    # Cloudinary
    CLOUDINARY_CLOUD_NAME=<your_cloudinary_cloud_name>
    CLOUDINARY_API_KEY=<your_cloudinary_api_key>
    CLOUDINARY_API_SECRET=<your_cloudinary_api_secret>

    # Stripe
    STRIPE_API_KEY=<your_stripe_api_key>
    STRIPE_WEBHOOK_SECRET=<your_stripe_webhook_secret>
    ```

5. Run the backend server:

    ```bash
    npm start
    ```

6. Your backend server should now be running at the specified port.

## Frontend Setup

1. Navigate to the frontend directory:

    ```bash
    cd frontend
    ```

2. Install frontend dependencies:

    ```bash
    npm install
    ```

3. Create a `.env` file based on `.env.example` and fill in the required environment variables:

    ```plaintext
    # API Base URL
    VITE_API_BASE_URL=<your_backend_api_base_url>

    # Auth0
    VITE_AUTH0_DOMAIN=<your_auth0_domain>
    VITE_AUTH0_CLIENT_ID=<your_auth0_client_id>
    VITE_AUTH0_CALLBACK_URL=<your_auth0_callback_url>
    VITE_AUTH0_AUDIENCE=<your_auth0_audience>
    ```

4. Run the frontend development server:

    ```bash
    npm run dev
    ```

5. Your React app should now be running and accessible at the specified URL.

## Additional Configuration

- To expand ESLint configuration, follow the instructions provided in the frontend `.env.example` file.
- Customize ESLint rules and TypeScript configurations according to your project's requirements.
- Update the `.gitignore` file as needed to exclude sensitive or unnecessary files from version control.

## Project Structure

- **Backend**: The backend directory contains all server-side code built with Express.js and TypeScript.
- **Frontend**: The frontend directory contains the React.js application with TypeScript.
- **Shared**: Shared code or utilities that can be used both in the backend and frontend can be placed here.

## Obtaining API Keys

### MongoDB Connection String

1. **Sign Up/Login to MongoDB**: If you don't have an account, sign up for MongoDB Atlas at [MongoDB Atlas](https://www.mongodb.com/cloud/atlas).
2. **Create a Cluster**: Once logged in, create a new cluster. Follow the prompts to choose your preferred cloud provider, region, and cluster settings.
3. **Get Connection String**: After your cluster is created, navigate to the "Clusters" section and click "Connect" on your newly created cluster. Follow the instructions to whitelist your IP address and create a MongoDB user. Once done, you'll get a connection string that includes your username, password, and other connection options.

### Auth0

1. **Sign Up/Login to Auth0**: If you haven't already, sign up for an account at [Auth0](https://auth0.com/).
2. **Create an Application**: Once logged in, navigate to the "Applications" section and create a new application. Choose the application type (e.g., Single Page Application) and configure the necessary settings.
3. **Get Client ID and Domain**: After creating the application, you'll get a Client ID and Domain. These will be used as `VITE_AUTH0_CLIENT_ID` and `VITE_AUTH0_DOMAIN` respectively in the frontend `.env` file.
4. **Set Allowed Callback URLs**: In your Auth0 application settings, set the allowed callback URLs to match your frontend URL (e.g., `http://localhost:5173`). This is important for authentication to work properly.

### Cloudinary

1. **Sign Up/Login to Cloudinary**: If you don't have an account, sign up for Cloudinary at [Cloudinary](https://cloudinary.com/).
2. **Get Cloud Name, API Key, and API Secret**: After logging in, navigate to your account dashboard or settings to find your Cloudinary cloud name, API key, and API secret. These will be used as `CLOUDINARY_CLOUD_NAME`, `CLOUDINARY_API_KEY`, and `CLOUDINARY_API_SECRET` respectively in the backend `.env` file.

### Stripe

1. **Sign Up/Login to Stripe**: If you don't have an account, sign up for Stripe at [Stripe](https://stripe.com/).
2. **Get Secret Key and Webhook Secret**: After logging in, navigate to the Developers > API keys section in the dashboard. Here, you'll find your secret key (`STRIPE_API_KEY`) and webhook secret (`STRIPE_WEBHOOK_SECRET`). Create a new webhook endpoint if needed and get the webhook secret.

Follow these steps to obtain the necessary API keys and secrets for the services used in the `.env` files. Make sure to keep these keys secure and never expose them publicly.

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

## Contributing

We welcome contributions to improve this project! Feel free to fork the repository, make your changes, and submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE).

## Acknowledgements

Special thanks to the creators and maintainers of the libraries, frameworks, and services used in this project. Without their hard work, this project wouldn't be possible.

# SIT737-2025-Prac6C

## Project Overview

This project is part of the SIT737 course, aimed at developing and implementing a real-world solution. The task involves integrating various technologies, managing version control, and deploying applications using Docker and Google Cloud Platform (GCP). This project demonstrates the full software development lifecycle from initial setup to deployment, as well as continuous integration and version control practices.

## Task Completion Overview

In this project, I completed the following tasks:

1. **Setting up Git Repository**:
   - Cloned the repository from GitHub and set up the local development environment.
   - Ensured synchronization between the local repository and the remote repository to avoid conflicts during development.

2. **Branch Management**:
   - Created and worked on a `feature-branch` to develop new features, avoiding conflicts with the `main` branch.
   - After completing the feature development, merged the `feature-branch` changes into the `main` branch and resolved merge conflicts.

3. **Containerization**:
   - Containerized the application using Docker to ensure consistency across different environments.
   - Created `Dockerfile` and `docker-compose.yml` files to build and run containers, setting up necessary services and port mappings.

4. **Google Cloud Deployment**:
   - Used Google Cloud Platform for deploying the application.
   - Configured Google Cloud Storage and Google Cloud Compute instances to ensure the application runs reliably in the cloud environment.

5. **Handling Merge Conflicts**:
   - When pulling from the remote repository, encountered unrelated history conflicts and resolved the issue by using the `--allow-unrelated-histories` option.
   - Ensured proper synchronization between the local and remote branches and manually resolved any conflicts.

6. **Testing and Continuous Integration**:
   - Set up a continuous integration pipeline to automatically build and deploy the application to Google Cloud whenever changes are pushed to the repository.
   - Implemented unit tests and integration tests to validate the functionality of the deployed application.

## Features

- **Git Version Control**: Used Git to track changes and ensure smooth development.
- **Containerized Application**: Used Docker to containerize the application, ensuring consistency across environments.
- **Google Cloud Deployment**: Deployed the application using Google Cloud services to ensure scalability and reliability.
- **CI/CD Integration**: Automated the build and deployment process using Google Cloud Build and Cloud Run.

## Tech Stack

- **Git**: Used for version control and tracking code changes.
- **Docker**: Used for containerizing the application to ensure environment consistency.
- **Google Cloud**: Used for cloud services and application deployment.
- **Node.js**: Used to build the backend of the application.
- **React**: Used to build the frontend user interface.
- **Google Cloud Build**: Used for automating the build and deployment process.

## Installation and Setup

To replicate the environment and run the application locally, follow these steps:

1. **Clone the repository to your local machine**:

    ```bash
    git clone https://github.com/CODEHAPP/sit737-2025-prac6c.git
    ```

2. **Navigate to the project directory**:

    ```bash
    cd sit737-2025-prac6c
    ```

3. **Install dependencies**:

    For the backend:

    ```bash
    npm install
    ```

    For the frontend:

    ```bash
    npm install
    ```

4. **Run the project**:

    For the backend:

    ```bash
    npm start
    ```

    For the frontend:

    ```bash
    npm start
    ```

5. **Access the application**:
    Open your browser and navigate to `http://localhost:3001` to view the application.

## Using Google Cloud for Deployment

1. **Install and configure the `gcloud` tool**:

    - Download and install the [Google Cloud SDK](https://cloud.google.com/sdk/docs/install).
    - Log in to Google Cloud:

    ```bash
    gcloud auth login
    ```

    - Set the project ID:

    ```bash
    gcloud config set project PROJECT_ID
    ```

2. **Configure Google Cloud Storage**:

    - Create a storage bucket:

    ```bash
    gcloud storage buckets create gs://your-bucket-name
    ```

    - Upload a file to the storage bucket:

    ```bash
    gcloud storage cp local-file.txt gs://your-bucket-name/
    ```

3. **Deploy to Google Cloud App Engine**:

    - Navigate to the directory containing your `app.yaml` configuration file and run the following command:

    ```bash
    gcloud app deploy
    ```

4. **Access the application**:

    - Once deployed, access the application using the following command:

    ```bash
    gcloud app browse
    ```

## Contributing

Feel free to submit issues and pull requests. All contributions will be reviewed and merged based on the project requirements.

## License

MIT License - See the [LICENSE](LICENSE) file for details.

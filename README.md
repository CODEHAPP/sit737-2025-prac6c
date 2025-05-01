# SIT737-2025-Prac6C

## Project Overview

This project is part of the SIT737 course and focuses on developing and implementing a practical solution. The task involves integrating various technologies, managing code versions, and deploying the application using Docker and Azure. This project demonstrates the full software development lifecycle, from initial setup to deployment, as well as continuous integration and version control practices.

## Task Completion Overview

In this project, I worked on the following tasks:

1. **Setting up the Git repository**: 
   - I cloned the repository from GitHub and set up the local environment.
   - Ensured the repository was synchronized with the remote to avoid conflicts during development.

2. **Branch Management**:
   - Created and worked on a `feature-branch` for new features to avoid conflicts with the `main` branch.
   - Merged changes from the `feature-branch` to `main` after completing the new features and resolving any merge conflicts.

3. **Dockerization**:
   - Containerized the application using Docker to ensure consistency across different environments.
   - Created `Dockerfile` and `docker-compose.yml` for building and running the containers, including setting up the necessary services and port mappings.

4. **Azure Deployment**:
   - Integrated the project with Azure to deploy the application in a cloud environment.
   - Configured an Azure Container Registry (ACR) and pushed the Docker images to it.
   - Used Azure services like Azure Kubernetes Service (AKS) for orchestrating container deployment and management.

5. **Handling Merge Conflicts**:
   - Faced challenges with unrelated histories when pulling from the remote repository, which were resolved using the `--allow-unrelated-histories` option in Git.
   - Ensured that both local and remote branches were synchronized correctly by resolving any conflicts manually.

6. **Testing and Continuous Integration**:
   - Set up continuous integration pipelines to automatically build and deploy the application to Azure when changes are pushed to the repository.
   - Implemented unit tests and integration tests to verify the functionality of the deployed application.

## Features

- **Version Control with Git**: Integrated Git for tracking changes and ensuring smooth collaboration.
- **Containerized Application**: Dockerized the application to run consistently across different environments.
- **Azure Deployment**: Deployed the application using Azure services for scalability and reliability.
- **CI/CD Integration**: Automated the build and deployment process using Azure Pipelines.

## Tech Stack

- **Git**: For version control and tracking changes in code.
- **Docker**: For containerizing applications and ensuring environment consistency.
- **Azure**: For cloud services, application deployment, and management.
- **Node.js**: For building the backend of the application.
- **React**: For building the frontend user interface.
- **Azure Pipelines**: For setting up continuous integration and deployment pipelines.

## Installation and Setup

To replicate the environment and run the application locally, follow these steps:

1. Clone the repository to your local machine:

    ```bash
    git clone https://github.com/CODEHAPP/sit737-2025-prac6c.git
    ```

2. Navigate into the project directory:

    ```bash
    cd sit737-2025-prac6c
    ```

3. Install dependencies:

    For the backend:

    ```bash
    npm install
    ```

    For the frontend:

    ```bash
    npm install
    ```

4. Run the project:

    For the backend:

    ```bash
    npm start
    ```

    For the frontend:

    ```bash
    npm start
    ```

5. Open your browser and visit `http://localhost:3001` to view the application.

## Contributing

Feel free to submit issues and pull requests. All contributions will be reviewed and merged based on project requirements.

## License

MIT License - See [LICENSE](LICENSE) for details.

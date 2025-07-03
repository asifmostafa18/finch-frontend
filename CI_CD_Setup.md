CI/CD Pipeline Setup

Overview
I am using GitHub Actions for CI/CD pipelines for both frontend and backend applications.

Pipeline Stages
Build and Test
   - Checks out code
   - Sets up Node.js environment
   - Installs dependencies
   - Runs tests
   - Performs linting

Build and Push Docker Image
   - Builds Docker image
   - Pushes to Docker Hub

How to Use
- Pipelines automatically run on push to `main` branch or pull requests
- Monitor pipelines in GitHub Actions tab
- Docker Hub credentials must be set as repository secrets:
  - `DOCKER_HUB_USERNAME`
  - `DOCKER_HUB_TOKEN`
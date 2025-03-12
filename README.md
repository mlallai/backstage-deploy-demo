# 🎬 Backstage Demo

### 🚀 Step 1: Local Deployment

#### 📋 Prerequisites

- 🐳 Docker installed

#### 🛠️ Instructions

1. 📄 Copy the example environment file:

   ```sh
   cp .env.example .env
   ```

   Optionally, if not using Docker:

   ```sh
   cp .env.yarn.example .env.yarn
   ```

2. 🔑 Create a GitHub OAuth App. Follow [this link](https://github.com/settings/applications/new) to create the app. Retrieve the `GITHUB_CLIENT_ID`, `GITHUB_CLIENT_SECRET`, and `GITHUB_USERNAME` from GitHub and paste the values into the `.env` and `.env.yarn` files.

3. 📂 Navigate to the `backstage-app` directory and run:
   ```sh
   cd backstage-app
   docker-compose up --build -d
   ```
4. 🌐 Open your browser and go to [http://localhost:7007](http://localhost:7007).

### 🌐 Step 2: Local Kubernetes Deployment

#### 📋 Prerequisites

- 🐳 Minikube installed ([installation guide](https://minikube.sigs.k8s.io/docs/start/))
- 📦 kubectl installed ([installation guide](https://kubernetes.io/docs/tasks/tools/install-kubectl/))

#### 🛠️ Instructions

1. 📜 Run the deployment script:

   ```sh
   sh deploy.sh
   ```

2. 🌐 Open your browser and go to the testing URL provided by the Kubernetes service.

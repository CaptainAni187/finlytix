# Finlytix: Personal Finance Dashboard with ML Forecasting

[![Frontend](https://img.shields.io/badge/Frontend-React-61DAFB?logo=react&logoColor=white)](https://reactjs.org/)
[![Backend](https://img.shields.io/badge/Backend-Python-3776AB?logo=python&logoColor=white)](https://www.python.org/)
[![Cloud](https://img.shields.io/badge/Cloud-GCP-4285F4?logo=google-cloud&logoColor=white)](https://cloud.google.com/)
[![Containerization](https://img.shields.io/badge/Container-Docker-2496ED?logo=docker&logoColor=white)](https://www.docker.com/)
[![ML](https://img.shields.io/badge/ML-Scikit--learn-F7931E?logo=scikit-learn&logoColor=white)](https://scikit-learn.org/)

**Finlytix** is a dashboard-based web application for visualizing and forecasting personal spending trends. It uses machine learning to provide financial insights from public transaction datasets. The project features secure user authentication, customizable budget alerts, and scalable data synchronization pipelines built with Python, React, Google Cloud Platform (GCP), and Docker.

---

## Table of Contents
- [Key Features](#key-features)
- [How It Works](#how-it-works)
- [System Architecture](#system-architecture)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [Usage](#usage)
- [Development](#development)
- [Contributing](#contributing)
- [Author](#author)

---

## Key Features
- **Interactive Dashboard**: Visualize spending habits, income vs. expenses, and net worth with interactive charts.
- **ML-Powered Forecasting**: Predict future spending patterns and get ahead of your finances.
- **Secure User Authentication**: Safe and secure login using Google Cloud Identity Platform.
- **Custom Budget Alerts**: Set spending limits and receive automated notifications.
- **Data Synchronization**: Automated pipelines to keep your financial data up-to-date.
- **Containerized Deployment**: Easily deploy and scale the application with Docker.

---

## How It Works
1. **Authentication**: Users securely log in via GCP Identity Platform.
2. **Data Ingestion**: Transaction data is imported from public datasets or manual uploads.
3. **Data Processing**: A Python backend processes and categorizes transactions.
4. **ML Analysis**: Forecasting models analyze historical data to predict future spending.
5. **Visualization**: The React frontend presents the data through an intuitive dashboard.
6. **Alerts**: A notification system sends budget alerts based on user-defined rules.

---

## System Architecture
Finlytix is built with a modern, scalable architecture:

1. **Python Backend (`/backend`)**:
    - **FastAPI**: For creating high-performance REST APIs.
    - **Scikit-learn/Statsmodels**: For machine learning and statistical modeling.
    - **Pandas**: For data manipulation and analysis.
2. **React Frontend (`/frontend`)**:
    - **React**: For building a dynamic and responsive user interface.
    - **Recharts/D3.js**: For creating interactive data visualizations.
    - **Axios**: For communicating with the backend API.
3. **Google Cloud Platform (GCP)**:
    - **Identity Platform**: For managing user authentication.
    - **Cloud Run/Kubernetes Engine**: For deploying the containerized application.
    - **Cloud SQL/Firestore**: For database and data storage needs.
4. **Docker**:
    - **Dockerfile**: To containerize the Python backend and React frontend.
    - **Docker Compose**: For managing multi-container local development.

---

## Getting Started

### Prerequisites
-   [Python](https://www.python.org/downloads/) (version 3.9 or higher)
-   [Node.js](https://nodejs.org/) (version 16 or higher) and npm
-   [Docker](https://www.docker.com/products/docker-desktop)
-   [Google Cloud SDK](https://cloud.google.com/sdk/docs/install)
-   [Git](https://git-scm.com/)

### Installation

1. **Clone the repository:**
    ```
    git clone https://github.com/CaptainAni187/meshfs-p2p-file-system.git
    cd meshfs-p2p-file-system
    ```
2. **Set up the Python backend:**
    ```
    # Create and activate a virtual environment
    python3 -m venv .venv
    source .venv/bin/activate
    # Install dependencies
    pip install -r requirements.txt
    ```
3. **Set up the React frontend:**
    ```
    cd frontend
    npm install
    ```

---

## Usage

1. **Configure Environment Variables**:
    - Create a `.env` file in the root directory and add your GCP credentials and any other necessary configurations for secure authentication, database, and API integration.
2. **Run the application with Docker Compose**:
    ```
    docker-compose up --build
    ```
3. **Access the application**:
    - Open your web browser and navigate to `http://localhost:3000`.

---

## Development

- The Python backend is modular, allowing for easy expansion of ML models and API endpoints.
- The React frontend uses a component-based architecture for easy maintenance and scalability.
- Run backend tests with `pytest`.
- Linting and formatting are enforced using `black` and `flake8` for Python, and `ESLint`/`Prettier` for the frontend.

---

## Contributing

Contributions are welcome! Please feel free to open an issue or submit a pull request for:
- Bug fixes
- New features (e.g., additional data source integrations, more advanced ML models)
- Improved documentation
- UI/UX enhancements

---

## Author

**Animesh (CaptainAni187)**
- **GitHub**: [CaptainAni187](https://github.com/CaptainAni187)
- **Project Repository**: [meshfs-p2p-file-system](https://github.com/CaptainAni187/meshfs-p2p-file-system)

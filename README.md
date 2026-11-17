# Insighta
### Non-Life Insurance AI Complaint Ticketing System

Insighta is an AI-powered complaint ticketing system designed for the non-life insurance industry. It aims to streamline complaint management by leveraging Natural Language Processing (NLP) and intelligent automation to process, analyze, and organize customer complaints.

The platform provides a centralized environment for handling insurance-related complaints, helping improve operational efficiency, reduce manual processing, and support faster complaint assessment and resolution.

## Key Features

- **AI-Powered Complaint Processing** – Uses NLP to analyze and process submitted complaints.
- **Automated Ticketing** – Facilitates the creation and organization of complaint tickets.
- **Intelligent Complaint Classification** – Helps categorize complaints based on their content.
- **Centralized Complaint Management** – Provides a unified platform for monitoring and managing complaints.
- **Background NLP Processing** – Runs a dedicated worker loop to handle NLP-related tasks asynchronously.
- **REST API Integration** – Uses FastAPI to handle backend operations and communication between system components.

## System Architecture

Insighta consists of three primary components:

| Component | Description |
|---|---|
| Frontend | Provides the user interface and application interactions. |
| Backend API | Handles backend logic and exposes RESTful endpoints through FastAPI. |
| NLP Worker | Processes NLP-related tasks through a background worker loop. |

## Technology Stack

- **Frontend:** Node.js, npm
- **Backend:** Python, FastAPI
- **AI / NLP:** Natural Language Processing
- **Communication:** RESTful API
- **Background Processing:** NLP Worker Loop

*Note: Update this section with the specific frontend framework, NLP libraries, database, and AI models used in the implementation.*

## Prerequisites

Ensure the following are installed before running the application:

- Node.js
- npm
- Python
- pip
- Git

## Installation and Setup

### 1. Clone the Repository

```bash
git clone <repository-url>
cd Insighta
```

### 2. Install Frontend Dependencies

Navigate to the frontend directory:

```bash
cd frontend
npm install
```

### 3. Set Up Backend Dependencies

Navigate to the backend directory:

```bash
cd backend
```

Install the required Python dependencies using the project's dependency file, if available:

```bash
pip install -r requirements.txt
```

## Running the Application

Insighta requires three processes to run its development environment: the frontend development server, FastAPI backend, and NLP background worker.

### 1. Start the Frontend Development Server

Open a terminal:

```bash
cd frontend
npm run dev
```

### 2. Start the FastAPI Backend

Open a separate terminal from the project root:

```powershell
cd backend
.\run-fastapi.bat
```

This starts the FastAPI backend using the project's configured startup script.

### 3. Start the NLP Worker Loop

Open another terminal from the project root:

```bash
cd frontend
npm run nlp:worker:loop
```

This starts the background worker responsible for executing NLP-related processing tasks.

## Development Workflow

For local development, ensure all three processes are running simultaneously:

| Process | Command | Purpose |
|---|---|---|
| Frontend | `npm run dev` | Runs the development server. |
| Backend | `.\run-fastapi.bat` | Starts the FastAPI application. |
| NLP Worker | `npm run nlp:worker:loop` | Executes background NLP processing. |

## Project Structure

```text
Insighta/
│
├── frontend/
│   ├── package.json
│   └── ...
│
├── backend/
│   ├── run-fastapi.bat
│   ├── requirements.txt
│   └── ...
│
└── README.md
```

## Project Objectives

Insighta aims to demonstrate the practical application of Artificial Intelligence and software engineering in the insurance industry through:

- Intelligent complaint processing and classification.
- Automation of complaint ticketing workflows.
- Integration of AI and NLP into business processes.
- Asynchronous background task execution.
- RESTful API-based application architecture.
- Improved organization and management of customer complaints.


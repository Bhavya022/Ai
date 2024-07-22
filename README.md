# Ai
# AI-Powered Content Summarization and Analysis Tool

## Overview

This project is an AI-powered content summarization and analysis tool that provides users with a user-friendly interface for uploading text content, integrating with an AI service for summarization and analysis, and displaying the results. It is built using Next.js for the frontend and Node.js with Express.js for the backend.

## Features

- **Text Summarization**: Summarizes the uploaded text content.
- **Sentiment Analysis**: Analyzes the sentiment of the text and provides insights.
- **Text Classification**: Classifies the text into predefined categories.
- **Keyword Extraction**: Extracts important keywords from the text.
- **Text Paraphrasing**: Provides a paraphrased version of the text.
- **Text-to-Speech**: Converts text to speech.
- **User Authentication**: Ensures only authenticated users can access the tool.
- **File Upload**: Supports uploading various text formats including PDF, TXT, HTML, DOC, and DOCX.
- **Report Download**: Allows users to download a summary report of the analysis.

## Tech Stack

- **Frontend**: Next.js
- **Backend**: Node.js, Express.js
- **AI Service**: Cohere API (for text summarization, sentiment analysis, etc.)

## Setup and Installation

### Prerequisites

- Node.js (v14.x or higher)
- npm or yarn
- Cohere API Key

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/ai-content-summarization.git
   cd ai-content-summarization
Install the dependencies for the backend:

```bash
cd backend
npm install
Install the dependencies for the frontend:

```bash
cd ../frontend
npm install
Configuration
Create a .env file in the backend directory with the following content:

env
COHERE_API_KEY=your_cohere_api_key
JWT_SECRET=your_jwt_secret
Create a .env.local file in the frontend directory with the following content:

env
NEXT_PUBLIC_API_URL=http://localhost:8000
Running the Application
Start the backend server:

bash
Copy code
cd backend
npm start
The backend server will run on http://localhost:8000.

Start the frontend development server:

bash

cd ../frontend
npm run dev
The frontend development server will run on http://localhost:3000.

Usage
Open your browser and navigate to http://localhost:3000.
Sign up or log in to access the tool.
Upload a text file or paste text to get a summary and analysis.
Download the summary report if needed.
API Endpoints
Backend Endpoints
POST /api/signup: User signup
POST /api/login: User login
POST /api/upload: Upload text file for summarization and analysis
GET /api/download-report: Download summary report
Frontend Pages
/: Main page with file upload and text analysis options
/login: Login page
/signup: Signup page
/summarizer: Text summarization page
/paraphraser: Text paraphrasing page
Contributing
Fork the repository.
Create a new branch (git checkout -b feature-branch).
Make your changes.
Commit your changes (git commit -m 'Add some feature').
Push to the branch (git push origin feature-branch).
Create a new Pull Request.

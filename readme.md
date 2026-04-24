# Node.js API Project

A lightweight, containerized REST API built with Node.js and Express. This project includes a health-check endpoint and is fully configured for git integration.

## 📁 Project Structure

```text
nodejs-api/
├── index.js           # Express server logic
├── node_modules         # Dnodes modules
├── docker-compose.yml # Container orchestration
├── package.json       # Dependencies and scripts
└── .gitignore         # Files excluded from Git

🚀 Quick Start (Local)

    Initialize and Install:
    Bash

    npm init -y
    npm i express
    npm i -D @types/express

    Create index.js:
    JavaScript

    const express = require('express');
    const app = express();
    const PORT = 8080;

    app.get('/health', (req, res) => {
        res.status(200).json({ status: "OK" });
    });

    app.listen(PORT, () => {
        console.log(`Server running on http://localhost:${PORT}`);
    });

    Run the App:
    Bash

    node index.js

📡 API Endpoints
Method	Endpoint	Description	Expected Response
GET	/health	Health Check	{"status": "OK"}

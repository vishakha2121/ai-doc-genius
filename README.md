# 🚀 AI Infrastructure Documentation Platform

<div align="center">

![AI Infrastructure Documentation Platform](https://img.shields.io/badge/AI-Infrastructure%20Documentation-purple?style=for-the-badge)
![React](https://img.shields.io/badge/React-18.2.0-blue?style=flat-square&logo=react)
![FastAPI](https://img.shields.io/badge/FastAPI-0.104.0-green?style=flat-square&logo=fastapi)
![Python](https://img.shields.io/badge/Python-3.10+-yellow?style=flat-square&logo=python)
![Gemini](https://img.shields.io/badge/Gemini-AI-orange?style=flat-square&logo=google)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

**Automatically document Kubernetes, Terraform, APIs, and CI/CD pipelines using AI**

[Features](#features) • [Tech Stack](#tech-stack) • [Quick Start](#quick-start) • [Architecture](#architecture) • [Screenshots](#screenshots) • [Contributing](#contributing)

</div>

---

## 📋 Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Architecture](#architecture)
- [Quick Start](#quick-start)
- [Installation](#installation)
- [Configuration](#configuration)
- [Usage](#usage)
- [API Documentation](#api-documentation)
- [Database Schema](#database-schema)
- [Deployment](#deployment)
- [Testing](#testing)
- [Screenshots](#screenshots)
- [Future Enhancements](#future-enhancements)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgments](#acknowledgments)

---

## 📖 Overview

**AI Infrastructure Documentation Platform** is a cutting-edge full-stack web application that leverages **Google's Gemini AI** to automatically generate comprehensive, human-readable documentation for various infrastructure components. It eliminates the manual effort of documenting complex infrastructure code, saving DevOps and Cloud engineers hours of tedious work.

### 🎯 What It Does

| Infrastructure Type | Input | Output |
|---------------------|-------|--------|
| **Kubernetes** | YAML manifests | Pod descriptions, service details, deployment strategies |
| **Terraform** | HCL files | Resource definitions, provider configurations, module explanations |
| **REST APIs** | OpenAPI/Swagger files | Endpoint documentation, request/response schemas |
| **CI/CD Pipelines** | YAML/JSON | Pipeline steps, deployment strategies, environment variables |
| **Docker** | Dockerfile | Container architecture, image layers, build process |

### 💡 Problem It Solves

- ❌ **Manual documentation** is time-consuming and error-prone
- ❌ **Inconsistent documentation** across teams
- ❌ **Outdated documentation** due to infrastructure changes
- ❌ **Knowledge silos** when team members leave
- ❌ **Complex infrastructure** is hard to explain

### ✨ Solution

- ✅ **AI-powered automation** generates documentation instantly
- ✅ **Consistent format** across all infrastructure
- ✅ **Auto-updates** with infrastructure changes
- ✅ **Human-readable explanations** of complex configs
- ✅ **Centralized knowledge base** accessible to everyone

---

## 🌟 Features

### Core Features

#### 🤖 AI-Powered Generation
- Upload any infrastructure file (YAML, HCL, JSON, Dockerfile)
- Google Gemini AI analyzes and understands the code
- Generates professional Markdown documentation
- Creates diagrams and visual representations

#### 📂 Multi-Infrastructure Support


#### 🎨 Beautiful User Interface
- Modern, clean design with glass-morphism effects
- Dark/Light mode toggle
- Responsive for all devices (mobile, tablet, desktop)
- Smooth animations and transitions
- Intuitive navigation

#### 📊 Interactive Dashboard
- Real-time statistics (Total documents, Infra types)
- Recent activity timeline
- Quick access to recent documents
- Document status tracking
- API usage analytics

#### 📝 Document Management
- **Create:** Generate new documents from files
- **Read:** View detailed documentation
- **Update:** Edit and refine AI-generated docs
- **Delete:** Remove outdated documents
- **Version History:** Track document changes
- **Export:** Download as PDF, HTML, or Markdown

#### 🔍 Smart Search & Filtering
- Search across all documents
- Filter by infrastructure type
- Sort by date, name, or status
- Tag-based categorization

#### 🔐 Security & Authentication
- JWT-based authentication
- User registration and login
- Secure API key management
- Environment variable protection

### Additional Features

#### 📎 File Upload
- Drag & drop support
- Multiple file formats supported
- Progress indicators
- File validation

#### 📈 Analytics
- Document usage statistics
- Infrastructure type distribution
- AI generation success rate
- User activity tracking

#### 🌐 GraphRAG Integration
- Connect related documents
- Build knowledge graphs
- Cross-reference infrastructure components
- Intelligent document linking

#### 🔔 Notifications
- Document generation complete
- Error alerts
- Success confirmations
- System updates

---

## 🛠️ Tech Stack

### Frontend


---

## 🚀 Quick Start

### Prerequisites

Before you begin, ensure you have installed:

| Tool | Version | Check Command |
|------|---------|---------------|
| Node.js | v18+ | `node --version` |
| npm | v9+ | `npm --version` |
| Python | 3.10+ | `python --version` |
| Git | Latest | `git --version` |
| Docker (optional) | Latest | `docker --version` |

### 5-Minute Quick Setup

```bash
# 1. Clone the repository
git clone https://github.com/vishakha2121/ai-doc-genius.git
cd ai-doc-genius

# 2. Set up backend
cd backend
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt
cp .env.example .env
# Edit .env and add your GEMINI_API_KEY

# 3. Set up frontend
cd ../frontend
npm install
cp .env.example .env

# 4. Run the application
# Terminal 1 - Backend
cd backend
uvicorn app.main:app --reload --port 8000

# Terminal 2 - Frontend
cd frontend
npm run dev


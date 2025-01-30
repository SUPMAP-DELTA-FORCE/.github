# SUPMAP - Real-time Navigation System

Welcome to the **SUPMAP** project! This repository contains the complete source code for our real-time navigation application, developed for the fictitious company **Trafine**. The system provides real-time traffic updates, optimized routes, and incident reporting, with a strong focus on **scalability, security, and user experience**.

The SUPMAP project consists of three main repositories:
- [Backend](https://github.com/SUPMAP-DELTA-FORCE/supmap-backend.git)
- [Mobile App](https://github.com/SUPMAP-DELTA-FORCE/supmap-mobile-app.git)
- [Webapp](https://github.com/SUPMAP-DELTA-FORCE/supmap-webapp.git)
## 📖 Project Overview

The SUPMAP system enables users to navigate in real-time while receiving live traffic updates, accident alerts, and other road-related events. It allows users to report incidents and contribute to a collaborative driving experience.

The project consists of:
- **A mobile application** (Android) for navigation and real-time updates.
- **A web application** for administrative management and data visualization.
- **A backend service** that handles API requests, authentication, and database management.

## 🚀 Features

- **Real-time navigation with optimized routing**
- **Incident reporting (accidents, traffic jams, roadblocks, police controls, etc.)**
- **Community validation of alerts**
- **Integration with Mapbox for mapping services**
- **Firebase Authentication for secure login**
- **Azure for secure storage and API integration**
- **Statistical analysis and data visualization for traffic insights**

---

## 🏗️ Project Structure

| Component     | Technology Stack |
|--------------|-----------------|
| **Backend** | NestJS, PostgreSQL, Azure Storage, Firebase Auth, Mapbox API |
| **Mobile App** | Kotlin (Android), Firebase, Mapbox Navigation API |
| **Webapp** | Next.js, React, Material-UI, Supabase |

---

## ✅ Prerequisites

To set up and run the project locally, ensure you have the following installed:

1. **Node.js** (>= 16.x) & **npm** (>= 8.x)
2. **Docker** (for PostgreSQL and Azurite emulation)
3. **Android Studio** (for mobile app development)
4. **NestJS CLI** (for backend development)
5. **Environment Variables**: Setup your `.env` files

### Environment Variables
Each repository requires an `.env` file for configuration. You can request access to secrets management at [supmap-deltaforce@proton.me](mailto:supmap-deltaforce@proton.me).

---

## 🏃 Running the Project Locally

### Backend Setup
```sh
git clone git@github.com:SUPMAP-DELTA-FORCE/supmap-backend.git
cd supmap-backend
npm install
cp .env.example .env
npm run start:dev
```
Backend API should be available at `http://localhost:3000`

### Mobile App Setup
```sh
git clone git@github.com:SUPMAP-DELTA-FORCE/supmap-mobile-app.git
```
- Open **Android Studio** and load the project.
- Configure the `local.properties` file.
- Click **Run** to launch the application.

### Webapp Setup
```sh
git clone git@github.com:SUPMAP-DELTA-FORCE/supmap-webapp.git
cd supmap-webapp
npm install
cp .env.example .env.local
npm run dev
```
Frontend should be available at `http://localhost:3000`

---

## 🐳 Using Docker
To quickly set up the development environment, use **Docker Compose**:
```sh
docker-compose up -d
```
Services started:
- PostgreSQL (`localhost:5432`)
- Azurite (Azure Emulator) (`localhost:10000`)

To stop the services:
```sh
docker-compose down
```

---

## 🛠️ Deployment & Production Notes
- **Ensure secrets are managed securely** (avoid committing API keys in `.env` files)
- **Use a cloud database service** for scalability (e.g., Azure PostgreSQL, Supabase)
- **Deploy backend using Docker** to ensure a stable environment

---

## 📜 License
This project is licensed under the MIT License - see the [LICENSE](./LICENSE) file for details.

---

For more information, contact the development team at [[supmap-deltaforce@proton.me](mailto:supmap-deltaforce@proton.me)](mailto:supmap-deltaforce@proton.me).

**Happy Coding! 🚀**

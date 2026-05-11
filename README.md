# DSA-Lab & Enterprise Patterns Knowledge Base

Welcome to the DSA-Lab repository. This project serves as an interactive environment to visualize Data Structures and Algorithms, built upon a production-ready Full-Stack architecture. It is designed to be a template for enterprise system design.

## 🏗 System Architecture
* **Frontend:** React.js (Vite) + Zustand for state management. Managed via `pnpm`.
* **Backend:** .NET 8 (C#) Minimal API.

---

## 🚀 Local Developer Setup (A-Z)

To run this project locally, ensure you have the **.NET 8 SDK**, **Node.js (v18+)**, and **pnpm** installed.

### 1. Start the API (Backend Engine)
Navigate to the API directory and start the .NET hot-reload server:
\`\`\`bash
cd API/DSA-Lab
dotnet restore
dotnet watch run
\`\`\`
*Note the port the API is running on (e.g., `https://localhost:7123`). Ensure CORS in `Program.cs` allows the UI origin.*

### 2. Start the UI (Frontend Client)
Open a new terminal, navigate to the UI directory, install dependencies, and start Vite:
\`\`\`bash
cd UI
pnpm install
pnpm run dev
\`\`\`
*Access the interactive UI at `http://localhost:5173`.*

---

## 📂 Folder Structure Overview
* `/API` - Contains the .NET solution. Business logic, algorithm implementations, and HTTP endpoints.
* `/UI` - Contains the React client. Reusable components, API service layers, and state slices.

## 🚢 Deployment Roadmap
This repository is structured to eventually support standard CI/CD pipelines:
1. **Dockerization:** Multi-stage builds for both the .NET runtime and an Nginx-served React client.
2. **CI/CD:** GitHub Actions to run `dotnet test` and `pnpm build` on PRs.
3. **Cloud Hosting:** API deployment to Managed App Services (AWS/Azure) and UI deployment to global CDNs (Vercel/Netlify).# DSA-Lab
DSA-Lab

# earlyexit.fun 🏖️

A secure, cloud-native retirement countdown and planning tool designed to project investment growth, visualize time to financial freedom, and explore retirement strategies with the help of an AI-powered advisor.

## Project Status
🚧 **Currently in development** - 

Week 1: Infrastructure & Static Timer

## Tech Stack
- Frontend: React
- Backend: Python Flask
- Auth: AWS Cognito
- Hosting: AWS Amplify
- Database: DynamoDB
- AI: Amazon Bedrock
- Domain: Cloudflare DNS

## Development Setup
More details coming as we build...

## Deployment
Target URL: https://earlyexit.fun




XXXXXXXXXXXXXX
Full README file:

# earlyexit.fun 🏖️

A secure, cloud-native retirement countdown and planning tool designed to project investment growth, visualize time to financial freedom, and explore retirement strategies with the help of an AI-powered advisor.

---

## 🎯 Project Objective

The goal of this project is to:

- Build a password-protected site showing a countdown to your planned retirement date.
- Calculate and display expected portfolio growth based on 6.5% YoY compounding.
- Deploy a secure full-stack app using React (frontend) and Flask (backend).
- Use AWS Amplify for hosting and authentication (Cognito).
- Automate deployments via GitHub CI/CD.
- Integrate Amazon Bedrock to serve as a personalized “Retirement Advisor.”
- Use Cloudflare as DNS provider with a custom domain: `earlyexit.fun`.

---

## 🗺️ Learning Path & Timeline

### 🔧 Week 1: Infrastructure & Static Timer

- [X] Create `earlyexit.fun` GitHub repo  
- [ ] Static HTML + JS countdown to **Aug 12, 2033 @ 12:00 PM**
- [ ] Initialize AWS Amplify project
- [ ] Add Cognito-based auth (`amplify add auth`)
- [ ] Deploy with `amplify publish`
- [ ] Connect custom domain via Cloudflare (DNS setup)
- [ ] Enable HTTPS with Cloudflare SSL

---

### ⚛️ Week 2: React + Cognito Auth

- [ ] Scaffold React frontend (Create React App or Vite)
- [ ] Integrate Amplify Auth UI for login/signup/reset password
- [ ] Show countdown page only to authenticated users
- [ ] Convert static countdown into React component

---

### 🔁 Week 3: CI/CD + Polish

- [ ] Enable GitHub → Amplify deployment pipeline
- [ ] Configure GitHub Actions for backend deployment
- [ ] Add logout, user profile menu
- [ ] Polish UI (basic CSS or Tailwind)

---

### 📈 Week 4: Growth Calculator MVP

- [ ] Form input for current portfolio value
- [ ] Calculate projected value using: `FV = PV × (1 + 0.065)^years`
- [ ] Display result on page
- [ ] Optional: add basic bar or line chart

---

### 🧠 Week 5: Flask API Backend

- [ ] Set up Flask server
- [ ] Add `/api/calculate` route to process projections
- [ ] Validate Cognito JWT in requests
- [ ] Store user data in DynamoDB
- [ ] Deploy backend using App Runner or Lambda + API Gateway

---

### 💬 Week 6: AI Retirement Advisor (Amazon Bedrock)

- [ ] Add Retirement Advisor UI (simple chat interface)
- [ ] Send inputs (portfolio, retirement date) to Flask
- [ ] Flask invokes Amazon Bedrock (Claude or Titan) with custom prompt
- [ ] Display LLM-generated insights and planning suggestions
- [ ] Optional: allow saving of responses to user profile

---

## 📦 Stack Overview

| Component        | Technology                     |
|------------------|-------------------------------|
| Frontend         | React (Vite or CRA)           |
| Auth             | AWS Cognito (via Amplify)     |
| Hosting          | AWS Amplify                   |
| Backend          | Python Flask                  |
| DB               | DynamoDB (user data)          |
| LLM Integration  | Amazon Bedrock (LLM Advisor)  |
| CI/CD            | GitHub + Amplify + GitHub Actions |
| Domain           | Cloudflare                    |

---

## 🚀 Domain

**https://earlyexit.fun** – hosted via AWS Amplify, with DNS handled by Cloudflare.

---

## 🧠 Future Ideas

- Email summaries (using SES)
- Track net worth over time
- Contribution simulator (DCA modeling)
- Compare early vs. late retirement trade-offs
- Add export to PDF/CSV

---

Happy building 🧱💰
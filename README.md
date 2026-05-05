# DevPilot

AI-powered GitHub companion for startups. Automatic code reviews, PR summaries, and changelog generation on every merge.

## What it does

- Login with GitHub
- Connect any of your repos
- Get AI code reviews on every Pull Request automatically
- Auto-generated changelog entries on every merge
- View all reviews on a clean dashboard

## Tech Stack

- **Frontend** - Next.js + Tailwind CSS
- **Backend** - Python + FastAPI
- **AI** - Claude API (Anthropic)
- **Auth** - GitHub OAuth
- **Webhooks** - GitHub Webhooks

## How it works

1. User logs in with GitHub
2. Selects a repo to connect
3. GitHub webhook is registered on that repo
4. Developer opens a PR on that repo
5. GitHub sends PR data to the backend
6. Backend fetches the code diff
7. Claude reviews the code automatically
8. Review is stored and displayed on the dashboard

## Getting Started

### Prerequisites
- Python 3.9+
- Node.js 18+
- GitHub OAuth App
- Anthropic API Key

### Backend Setup
```bash
cd backend
pip install -r requirements.txt

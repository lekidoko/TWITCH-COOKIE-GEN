# Twitch Cookie Token Generator

A Vercel-deployed API that generates Twitch authentication cookies and tokens.

## Features
- Generate Twitch OAuth tokens
- Extract auth cookies from tokens
- Secure environment variable management
- Easy Vercel deployment

## Setup

### 1. Get Twitch Credentials
1. Go to [Twitch Developer Console](https://dev.twitch.tv/console/apps)
2. Create a new application
3. Copy your **Client ID** and **Client Secret**

### 2. Deploy to Vercel
```bash
npm install -g vercel
vercel
```

### 3. Set Environment Variables
- `TWITCH_CLIENT_ID`: Your Twitch Client ID
- `TWITCH_CLIENT_SECRET`: Your Twitch Client Secret

## Usage

Send a POST request:
```bash
curl -X POST https://your-project.vercel.app/api/generate \
  -H "Content-Type: application/json" \
  -d '{"username": "your_username", "password": "your_password"}'
```

## License
MIT
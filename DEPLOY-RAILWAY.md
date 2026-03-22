# Railway deployment instructions

## 1. Connect your repo to Railway
- Go to https://railway.app/
- Create a new project and link your GitHub repository.

## 2. Environment Variables
- Set any required environment variables in the Railway dashboard (Settings > Variables).
- Your app uses `process.env.PORT` (Railway sets this automatically).

## 3. Deploy
- Railway will auto-detect your Node.js app and use `npm start` (from package.json).
- You can customize build/start in `railway.json`.

## 4. Remove Heroku-specific code (optional)
- The Heroku keep-alive ping in server.js is not needed for Railway, but it won't break anything if left in.

## 5. Done!
- Your app will be deployed and accessible via the Railway-provided URL.

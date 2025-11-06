# my-mern-chatbot

Server notes

- Copy `.env.example` to `.env` and fill in your keys. Never commit `.env`.

Example `.env` values (PowerShell):

```powershell
#$env:OPENAI_KEY = 'sk-...'
# to persist for this project, create a file named .env with:
# OPENAI_KEY=sk-...
# MONGO_URI=mongodb+srv://<user>:<password>@cluster0.mongodb.net/mydb
# PORT=5000
```

Start server (from project root):

```powershell
# install dependencies
npm install
# run server (ensure .env has keys and MONGO_URI if you want DB)
node server/index.js
```

Security: keep your `OPENAI_KEY` secret. Use your hosting provider's secret manager for production.
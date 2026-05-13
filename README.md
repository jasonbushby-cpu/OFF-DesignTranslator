# Übersetz — One for Fun Translation Studio

## Deploy to Vercel

1. Push this folder to a GitHub repo
2. Import the repo in Vercel
3. Add environment variable in Vercel dashboard:
   - Key: `ANTHROPIC_API_KEY`
   - Value: your Anthropic API key (`sk-ant-…`)
4. Deploy — done!

## Project structure

```
/api/translate.js   ← Serverless proxy (hides the API key)
/public/index.html  ← The translation tool UI
/vercel.json        ← Routing config
.env.example        ← Copy to .env.local for local dev
```

## Local development

```bash
npm i -g vercel
cp .env.example .env.local
# Add your real key to .env.local
vercel dev
```

# Deploy `invoice.html` to Vercel

Quick steps to deploy this static project to Vercel.

1) Deploy with the Vercel CLI (recommended for quick test)

PowerShell:
```powershell
# install (optional) then run from project folder
npm i -g vercel
cd "d:\Mick\Invoice_project"
vercel        # follow prompts
vercel --prod # to deploy to production
```

Or without global install:
```powershell
npx vercel
```

2) Deploy via GitHub (recommended for continuous deploy)
- Create a Git repo in this folder and push to GitHub.
- In the Vercel dashboard choose "Import Project" → select the Git repo → Deploy.

Notes
- Current file is `invoice.html`. The included `vercel.json` rewrites `/` to `/invoice.html`, so your site root will show the invoice.
- If you prefer the root to be `index.html`, rename `invoice.html` to `index.html` before deploying.
- If you want me to push to a new GitHub repo or help configure the Vercel project, tell me and I can create the repo and show exact commands.

# UHH DIRT // GROW — tracker (grow.uhhdirt.com)

Standalone React grow tracker, Field Manual skin. Saves to the browser's localStorage.
Deploys independently from the main UHH DIRT static site.

## Run locally
```
npm install
npm run dev
```

## Deploy to grow.uhhdirt.com (Vercel)
1. Push this folder to its own GitHub repo (e.g. `uhhdirt-grow`).
2. Import the repo at vercel.com → Deploy (Vite auto-detected).
3. In Vercel → Settings → Domains, add `grow.uhhdirt.com`.
4. In GoDaddy DNS, add a CNAME: host `grow` → value `cname.vercel-dns.com`.
5. HTTPS auto-issues once DNS resolves.

Separate from the main `uhhdirt` repo by design — keeps the art site clean and static.

## Notes
- Data is per-device (localStorage), not a shared database.
- Edit the SOP data at the top of `src/GrowTracker.jsx`.

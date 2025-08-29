[README.md](https://github.com/user-attachments/files/22052185/README.md)
# Raising Daisies – Deploy Bundle

Three ways to launch to your iPhone. Push this repo to GitHub, then click a button below.

## 1) One‑Click App (Next.js + API + PWA) — recommended
Works instantly with sample data. If you connect **Vercel Postgres**, it upgrades automatically.

**Deploy to Vercel:**  
https://vercel.com/new/clone?repository-url={REPO_URL}/tree/main/oneclick

**Open on iPhone:**  
Visit your Vercel URL in Safari → Share → *Add to Home Screen*.

**QR page:**  
After deploy, open: `/qr` (e.g., `https://YOUR-URL/qr`) — it shows a scannable QR for easy sharing.

---

## 2) Instant App (no backend) — fastest
Static PWA with sample events; works offline.

**Deploy to Vercel:**  
https://vercel.com/new/clone?repository-url={REPO_URL}/tree/main/instant

**Open on iPhone:**  
Visit your Vercel URL in Safari → Share → *Add to Home Screen*.

---

## 3) Full Backend (FastAPI on Railway) + Frontend (Vercel)
When you’re ready for real submissions/approvals, deploy the backend and point the frontend at it.

**Deploy backend to Railway:**  
Create a new Railway project from `/backend`, add a Postgres plugin, set `DATABASE_URL`, optional `ADMIN_TOKEN`, and deploy.

**Then** set your frontend’s `NEXT_PUBLIC_API_BASE` to your Railway backend URL (you can use the One‑Click app as the frontend by setting this env var in Vercel).

---

## iPhone install steps
1. Open your deployed URL in **Safari**.  
2. Tap **Share** → **Add to Home Screen** → **Add**.  
3. Launch from your home screen for a full‑screen, app‑like experience.

> Crisis support: Call/Text/Chat **988** (shown in footer).

---

## Repo contents
- **/oneclick** — Next.js + API + PWA (recommended starting point)
- **/instant** — static PWA (no backend)
- **/backend** — FastAPI + Docker + Railway config

---

**Note:** Replace `{REPO_URL}` in the Vercel links above with your GitHub repo URL after you push this bundle.

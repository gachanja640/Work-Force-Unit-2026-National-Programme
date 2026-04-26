# WFU Kenya — National Workforce Development Portal
## wfu.go.ke

**Work Force Unit | Republic of Kenya | 2025**

A fully functional, eCitizen-themed web portal for Kenya's national workforce development and infrastructure acceleration programme.

---

### 🌍 Live Portal
Deploy to GitHub Pages → your URL will be: `https://[your-username].github.io/wfu-kenya`

For the official domain **wfu.go.ke**, point your domain's DNS to GitHub Pages after deployment.

---

### 📋 Features

| Module | Description |
|--------|-------------|
| **Public Home** | Programme stats, live project summary, service portal grid |
| **Public Tracker** | Projects, fund disbursements, contracts register, group deployments — all publicly visible |
| **Member Account** | Personal dashboard with training milestones, skill portfolio, certificates |
| **Certificates** | TVET-accredited certificate display and download per member |
| **Apply / Join** | Full application form for WFU Phase 1 intake |
| **About / Proposal** | Programme overview + guidance on proposing to ministries/State House |

---

### 🚀 Deploy to GitHub Pages (No API Needed)

**Step 1 — Create repo**
```bash
git init
git add .
git commit -m "Initial WFU portal deployment"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/wfu-kenya.git
git push -u origin main
```

**Step 2 — Enable GitHub Pages**
1. Go to your repo → **Settings** → **Pages**
2. Under **Source**, select **GitHub Actions**
3. The `.github/workflows/deploy.yml` file handles the rest automatically

**Step 3 — Your site goes live at:**
`https://[your-username].github.io/wfu-kenya`

---

### 🌐 Custom Domain (wfu.go.ke)

To use a custom `.go.ke` domain:
1. Add a `CNAME` file to this repo containing: `wfu.go.ke`
2. In GitHub Pages settings, enter `wfu.go.ke` as the custom domain
3. At your domain registrar / Kenya ICT Authority DNS, add:
   - **CNAME record**: `www` → `[your-username].github.io`
   - **A records** (for apex domain): point to GitHub Pages IPs:
     - `185.199.108.153`
     - `185.199.109.153`
     - `185.199.110.153`
     - `185.199.111.153`

---

### 📁 File Structure
```
wfu-kenya/
├── index.html          ← Full portal (single-file)
├── README.md
└── .github/
    └── workflows/
        └── deploy.yml  ← Auto-deploy on push
```

---

### 🏛️ About WFU
The Work Force Unit is a private-led national infrastructure delivery mechanism targeting 5,000 Kenyan youth aged 25–35. Programme aligned with Kenya's Bottom-Up Economic Transformation Agenda and Vision 2030.

**Contact:** info@wfu.go.ke | 0800 723 456

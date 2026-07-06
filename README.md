# Momin Ali Khan — Portfolio

A single-page personal portfolio (mechanical · aerospace · automation engineering). Pure HTML/CSS/JS — no build step, no dependencies. Loads instantly and works on mobile.

---

## 1. Put your files in place

```
Git hub expert/
├── index.html
├── README.md
└── assets/
    ├── Momin_Ali_Khan_CV.pdf              ← your resume (for the "Download CV" button)
    └── solidworks-cswa-certificate.pdf    ← your SOLIDWORKS certificate
```

Create the `assets` folder and drop those two files in. (The site works without them, but the CV/certificate buttons will 404 until they exist.)

## 2. Fill in your personal links

Open `index.html` and replace these placeholders (each is marked with an HTML comment):

| Placeholder | Where | Replace with |
|---|---|---|
| `YOUR-LINKEDIN` | Contact section | your LinkedIn profile handle |
| `assets/Momin_Ali_Khan_CV.pdf` | Hero button | your actual CV filename |
| `assets/solidworks-cswa-certificate.pdf` | Certifications | your actual certificate filename |

Your email (`mominalikhan42@gmail.com`) and GitHub (`koolkingisone`) are already wired in.

## 3. Publish for free with GitHub Pages

Your account is **koolkingisone**, so your site will be live at **https://koolkingisone.github.io**.

1. Go to <https://github.com/new>.
2. Name the repository **exactly** `koolkingisone.github.io`. Set it to **Public**. Click **Create repository**.
3. On the new empty repo page, click **uploading an existing file**.
4. Drag in `index.html` and the whole `assets` folder. Commit.
5. Go to **Settings → Pages**. Source = **Deploy from a branch**, Branch = **main**, folder = **/ (root)**. Save.
6. Wait ~1 minute, then open **https://koolkingisone.github.io** — you're live.

**Prefer the command line?** From this folder:

```bash
git init
git add .
git commit -m "Initial portfolio"
git branch -M main
git remote add origin https://github.com/koolkingisone/koolkingisone.github.io.git
git push -u origin main
```

Then enable Pages in Settings → Pages as above.

## 5. Optional — custom domain

In **Settings → Pages → Custom domain**, add e.g. `mominalikhan.com` (buy it from any registrar), then add the DNS records GitHub shows you. Free HTTPS is issued automatically.

---

### Editing tips
- All content lives in `index.html`. Search for a heading (e.g. "Remote Control Weapon Station") to find and edit any section.
- Colours/theme are the `:root` variables at the top of the `<style>` block — change `--accent` to re-skin the whole site.
- Add a project by copying one `<article class="card reveal">…</article>` block.

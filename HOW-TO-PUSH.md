# How to Update & Publish Your Portfolio

Your live site: **https://koolkingisone.github.io/**
All content is in one file: **index.html** (in this folder).

---

## The 3-step routine every time you edit

1. **Edit** `index.html` in any text editor (VS Code, Notepad++, or Notepad). Save the file.
2. **Open PowerShell in this folder.** Easiest way: open this folder in File Explorer, click the address bar, type `powershell`, press Enter.
3. **Run these 4 commands** (copy–paste the whole block):

```powershell
cd "D:\github\Git hub expert"
git add .
git commit -m "Update portfolio"
git push
```

Wait 1–2 minutes, then hard-refresh your site (**Ctrl + F5**) to see the changes.

> Tip: change the message in quotes each time to describe what you changed, e.g. `git commit -m "Add new project"`.

---

## Adding your files (CV, certificate, photo)

Drop these into the **assets** folder, then run the 4 commands above to publish:

| File to add | Filename it must have | Activates |
|---|---|---|
| Your resume | `Momin_Ali_Khan_CV.pdf` | "Download CV" button |
| SOLIDWORKS certificate | `solidworks-cswa-certificate.pdf` | Certification link |
| Your photo | `portrait.jpg` | Replaces the "MK" box in About* |

\*To show the photo, also change the About block in `index.html` from the "MK" placeholder to an image — or just ask Claude to do it.

---

## If a command fails

- **"git is not recognized"** — open a new PowerShell window (Git was installed; a fresh window picks it up).
- **Asked to log in when pushing** — a browser window opens; sign in as `koolkingisone` and approve. It only asks once.
- **Site didn't update** — GitHub's build can take a few minutes. Hard-refresh with Ctrl + F5. Check build status at: https://github.com/koolkingisone/koolkingisone.github.io/deployments

---

## Don't want to use commands?

Just tell Claude what to change (e.g. "change my headline to X" or "add a project about Y") and Claude will edit and push it for you.

---

## Quick reference

- **Live site:** https://koolkingisone.github.io/
- **Your repository:** https://github.com/koolkingisone/koolkingisone.github.io
- **File to edit:** `index.html`
- **Publish:** `git add .` → `git commit -m "..."` → `git push`

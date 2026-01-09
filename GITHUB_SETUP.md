# GitHub Authentication Issue - How to Fix

## Problem
Git is trying to push as `vivek-tester` but needs authentication for `Eternal0p/Iron-Heresy`.

## Solution Options

### Option 1: Using GitHub CLI (Recommended - Easiest)

1. **Install GitHub CLI** (if not installed):
   - Download from: https://cli.github.com/
   - Or via winget: `winget install GitHub.cli`

2. **Authenticate:**
   ```powershell
   gh auth login
   ```
   - Select "GitHub.com"
   - Select "HTTPS"
   - Authenticate via browser

3. **Push:**
   ```powershell
   git push -u origin main
   ```

---

### Option 2: Using Personal Access Token (Classic Method)

1. **Create a Personal Access Token:**
   - Go to: https://github.com/settings/tokens
   - Click "Generate new token" → "Generate new token (classic)"
   - Give it a name: "Iron Heresy Development"
   - Select scopes: `repo` (all repo permissions)
   - Click "Generate token"
   - **COPY THE TOKEN** (you won't see it again!)

2. **Update remote URL with token:**
   ```powershell
   git remote set-url origin https://YOUR_TOKEN@github.com/Eternal0p/Iron-Heresy.git
   ```
   Replace `YOUR_TOKEN` with the token you just generated.

3. **Push:**
   ```powershell
   git push -u origin main
   ```

---

### Option 3: Using SSH Key (Most Secure)

1. **Generate SSH key** (if you don't have one):
   ```powershell
   ssh-keygen -t ed25519 -C "your_email@example.com"
   ```
   Press Enter to accept defaults.

2. **Copy your public key:**
   ```powershell
   Get-Content ~/.ssh/id_ed25519.pub | clip
   ```

3. **Add to GitHub:**
   - Go to: https://github.com/settings/keys
   - Click "New SSH key"
   - Paste the key and save

4. **Change remote to SSH:**
   ```powershell
   git remote set-url origin git@github.com:Eternal0p/Iron-Heresy.git
   ```

5. **Push:**
   ```powershell
   git push -u origin main
   ```

---

### Option 4: Push via Browser Authentication

Some Git clients support browser-based OAuth. Make sure you're logged into GitHub in your browser, then try:

```powershell
git push -u origin main
```

Windows may prompt you for credentials via a browser window.

---

## Quick Command Reference

After authentication is set up:

```powershell
cd c:\Users\airbo\Desktop\Eternal\Iron-Heresy
git push -u origin main
```

---

## Current Status ✅

- ✅ Files committed locally
- ✅ Remote added: https://github.com/Eternal0p/Iron-Heresy.git
- ❌ Authentication needed to push

**Choose one of the options above to authenticate, then try pushing again!**

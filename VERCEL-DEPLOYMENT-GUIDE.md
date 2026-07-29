# 🚀 DEPLOY TO VERCEL - STEP BY STEP

**Time:** ~5 minutes  
**Cost:** FREE  
**Result:** Live URL like: `https://security-bank-transactions.vercel.app`

---

## STEP 1: PREPARE FILES

You need 3 files in a GitHub repository:

1. **index.html** ← The app (already provided)
2. **vercel.json** ← Vercel config (already provided)
3. **.gitignore** ← Git settings (optional)

---

## STEP 2: CREATE GITHUB REPOSITORY

1. Go to **https://github.com/new**
2. Repository name: `security-bank-transactions-cloud`
3. Description: `Multi-user Security Bank Transaction Management`
4. Choose **Public** (easier for Vercel)
5. Click **Create repository**

---

## STEP 3: UPLOAD FILES TO GITHUB

### Option A: Upload via GitHub Website (Easiest)

1. In your new repo, click **Add file** → **Upload files**
2. Download these 3 files:
   - `index.html`
   - `vercel.json`
   - Create `.gitignore` (empty file is fine)
3. Drag & drop them into GitHub
4. Click **Commit changes**

### Option B: Use Git Commands (Advanced)

```bash
git clone https://github.com/YOUR-USERNAME/security-bank-transactions-cloud.git
cd security-bank-transactions-cloud
# Copy index.html and vercel.json here
git add .
git commit -m "Initial commit: Security Bank app"
git push
```

---

## STEP 4: CONNECT TO VERCEL

1. Go to **https://vercel.com**
2. Click **Sign up** (or login if you have account)
3. Click **Continue with GitHub**
4. Authorize Vercel to access GitHub
5. Click **New Project**
6. Find your repo: `security-bank-transactions-cloud`
7. Click **Import**

---

## STEP 5: CONFIGURE VERCEL

**You should see a configuration page. Leave defaults:**
- Framework: None (static)
- Build Command: (leave empty)
- Output Directory: (leave empty)

**Click DEPLOY** ✅

---

## STEP 6: WAIT FOR DEPLOYMENT

Vercel will show:
- Building...
- Deploying...
- ✅ Ready!

**Once complete, you get a URL like:**
```
https://security-bank-transactions-cloud.vercel.app
```

---

## STEP 7: TEST THE APP

1. Click the **Visit** button (or copy the URL)
2. Try logging in with:
   - Email: `yamanatrucks@gmail.com`
   - Password: (the password you set in Supabase)
3. ✅ Should see the dashboard!

---

## STEP 8: SHARE THE LIVE URL

Send to your team:
```
https://security-bank-transactions-cloud.vercel.app
```

Both users can login with their Supabase credentials:
- `yamanatrucks@gmail.com`
- `work.ahmr@gmail.com`

---

## TROUBLESHOOTING

**Q: Getting 404?**
- Wait 2-3 minutes for deployment to complete
- Refresh browser (Ctrl+F5)

**Q: Can't login?**
- Make sure users exist in Supabase (Authentication → Users)
- Check password is correct

**Q: Data not saving?**
- Check Supabase credentials in the app code (they're already set)
- Make sure Supabase tables exist (run SQL schema first)

**Q: Want a custom domain?**
- In Vercel → Project Settings → Domains
- Add your own domain (requires DNS setup)

---

## NEXT STEPS

✅ Deploy to Vercel  
✅ Test with both users  
✅ Start using for real transactions  

**Need help? Let me know!**

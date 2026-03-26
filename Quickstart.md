# ⚡ Mubra AI - Quick Setup Guide

## 🎯 5-Minute Setup

### Step 1: Get Your Free API Key (2 minutes)

1. Open https://aistudio.google.com in your browser
2. Click **"Get API key"** button
3. Select **"Create API key in new project"**
4. Copy the API key shown
5. Keep this window open!

### Step 2: Configure the App (1 minute)

1. Open `mubra-chemistry-app.html` in a text editor
   - Windows: Right-click → "Open with" → Notepad
   - Mac: Right-click → "Open with" → TextEdit
   - Linux: Any text editor

2. Find this line (around line 564):
   ```javascript
   GEMINI_API_KEY: 'YOUR_GEMINI_API_KEY_HERE',
   ```

3. Replace with your actual key:
   ```javascript
   GEMINI_API_KEY: 'AIzaSyD_YourActualKeyHere_xxxxxxxxxxxxxxxx',
   ```

4. Save the file (Ctrl+S or Cmd+S)

### Step 3: Test It! (1 minute)

1. Double-click `mubra-chemistry-app.html`
2. Your browser opens the app
3. Click a lesson (e.g., "Organic Chemistry")
4. Type a question: "Explain benzene structure"
5. Click the send button (📤)
6. Wait for the AI response!

### Step 4: Deploy to GitHub Pages (1 minute)

**Option A: If you have Git installed**

```bash
# In your project folder
git init
git add mubra-chemistry-app.html README.md
git commit -m "Add Mubra AI Chemistry App"
git branch -M main

# Create GitHub repo first, then:
git remote add origin https://github.com/YOUR_USERNAME/mubra-chemistry.git
git push -u origin main
```

Then in GitHub Settings → Pages → Deploy from main → Save

**Option B: Without Git (GitHub Web UI)**

1. Go to https://github.com/new
2. Create repository named `mubra-chemistry`
3. Click "Create repository"
4. Click "uploading an existing file"
5. Drag `mubra-chemistry-app.html` and `README.md`
6. Click "Commit changes"
7. Go to Settings → Pages
8. Source: main branch
9. Click Save
10. Your app is live! (May take 1-2 minutes)

---

## 🔍 Verification Checklist

- [ ] API key is valid (test message works)
- [ ] App loads without errors
- [ ] Chat bubbles appear correctly
- [ ] KaTeX formulas render (e.g., $H_2SO_4$)
- [ ] Sinhala text displays properly
- [ ] Mobile view is responsive

---

## ❓ Common Issues & Quick Fixes

### "API key is not valid"
→ Check you copied the full key correctly  
→ Make sure no extra spaces at start/end  

### "No response from AI"
→ Check your internet connection  
→ Open browser console (F12) to see error  
→ Verify you haven't exceeded 15,000 daily requests  

### "Nothing happens when I click send"
→ Reload the page  
→ Check API key is configured  
→ Clear browser cache (Ctrl+Shift+Delete)  

### "Chemistry formulas show as code"
→ Page is loading KaTeX from internet  
→ Make sure you have internet connection  
→ Refresh the page  

---

## 🎓 Example Questions to Try

### Organic Chemistry
- "What is the mechanism of the SN2 reaction?"
- "Explain the structure of benzene"
- "How do you distinguish primary, secondary, and tertiary alcohols?"

### Inorganic Chemistry
- "What are the properties of d-block elements?"
- "Explain redox reactions with an example"
- "How is ammonia manufactured industrially?"

### Physical Chemistry
- "Calculate Kp for a gaseous equilibrium"
- "Explain Le Chatelier's principle"
- "How do you determine activation energy?"

### Past Papers
- "2020 paper, question 5: How would you prepare..."
- "What were the common mistakes in 2019 paper?"
- "Explain the marking scheme for this question"

---

## 💡 Tips for Best Results

1. **Be Specific**: Instead of "explain benzene", say "explain the structure of benzene using resonance theory"

2. **Reference Past Papers**: "2018 paper question 3: explain the mechanism of..."

3. **Ask Follow-ups**: If you don't understand, ask "Can you explain this part more simply?"

4. **Use Chemistry Notation**: Write formulas like $H_2SO_4$, $K_p$, etc.

5. **Learn Sinhala Responses**: The AI responds in Sinhala - this helps you learn Sinhala chemistry terminology!

---

## 🔐 Security Note

⚠️ Your API key is visible in the HTML source code. This is fine for:
- Learning projects
- Personal use
- Free tier testing

For production use, consider:
- Using a backend server to hide the key
- Environment variables
- OAuth authentication

---

## 📊 API Usage

**Free Tier:**
- 15,000 requests per day
- Each question = 1-2 requests
- Perfect for learning!

**After free tier:**
1. Upgrade to paid in Google Cloud Console
2. Set spending limits
3. Upgrade to better models (optional)

---

## 🎨 Customization Options

### Change Colors
Find `:root { --navy-primary: #001F3F; --gold-primary: #D4AF37; }`  
Edit the color codes

### Change AI Personality
Find `const SYSTEM_INSTRUCTION = '...'`  
Modify the Sinhala text

### Add More Lessons
Find `data-lesson="organic"` sections  
Duplicate and modify

---

## 📱 Mobile Optimization

The app is fully optimized for:
- ✅ iPhones and iPads
- ✅ Android phones
- ✅ Tablets
- ✅ Desktop computers

Just open the GitHub Pages link on any device!

---

## 🎯 Next Steps

1. ✅ Configure API key
2. ✅ Test locally
3. ✅ Deploy to GitHub Pages
4. ✅ Share with friends
5. ✅ Start learning chemistry!

---

## 📞 Need Help?

Check the main README.md for:
- Detailed feature descriptions
- Advanced customization
- Troubleshooting guide
- Educational resources

---

**Ready? Let's get started! 🚀**

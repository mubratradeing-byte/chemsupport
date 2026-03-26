# 🧪 Mubra AI 8.v1 - Sri Lankan A/L Chemistry Expert

A **premium, AI-powered educational application** designed for Sri Lankan G.C.E. A/L Chemistry students. Built with luxury aesthetics (Navy Blue & Gold), Sinhala language support, and advanced AI integration using Google Gemini API.

![Premium Chemistry Tutor](https://img.shields.io/badge/Premium-Educational%20Platform-gold)
![Chemistry](https://img.shields.io/badge/Chemistry-A%2FL%20Syllabus-blue)
![Sinhala Support](https://img.shields.io/badge/Language-Sinhala-red)

---

## ✨ Key Features

### 🎨 **Premium UI/UX Design**
- **Luxury Color Scheme**: Navy Blue (#001F3F) with Metallic Gold (#D4AF37)
- **Modern SPA Architecture**: Smooth, responsive single-page application
- **Elegant Sidebar Navigation**: Quick access to lessons and past papers (1985-2025)
- **Professional Typography**: Cormorant Garamond (display) + Lato (body)
- **Full Mobile Optimization**: Perfectly rendered on phones, tablets, and desktops

### 🧠 **AI-Powered Chemistry Expert**
- **Mubra AI 8.v1**: Legendary Sri Lankan chemistry guru personality
- **Sinhala-Only Responses**: Dedicated system prompt ensuring Sinhala medium instruction
- **Expertise Areas**:
  - ⚛️ **Organic Chemistry**: Mechanisms, synthesis, reactions
  - 🔬 **Inorganic Chemistry**: Properties, redox, coordination compounds
  - 📊 **Physical Chemistry**: Calculations, equilibrium, thermodynamics

### 📚 **Comprehensive Content Coverage**
- **Past Papers Archive**: Questions from 1985-2025 (41 years)
- **Lesson Organization**: Browse by topic (Organic, Inorganic, Physical)
- **Step-by-Step Guidance**: Detailed explanations for mechanisms and calculations
- **Marking Scheme Insights**: Analysis from past papers and exam trends

### 🧮 **Advanced Chemistry Notation**
- **KaTeX Integration**: Professional rendering of chemical formulas
  - Molecular formulas: $H_2SO_4$, $CuSO_4 \cdot 5H_2O$
  - Equilibrium constants: $K_p$, $K_c$, $K_a$
  - Thermodynamic symbols: $\Delta H°$, $\Delta G°$, $\Delta S°$
- **Unicode Sinhala Support**: Perfect rendering of Sinhala text

---

## 🚀 Quick Start Guide

### Step 1: Get Your Google Gemini API Key

1. Go to **[Google AI Studio](https://aistudio.google.com/)**
2. Click **"Get API Key"** → **"Create API key in new project"**
3. Copy your API key (keep it secure!)
4. The API key is **free** for up to 15,000 requests per day

### Step 2: Configure the Application

Open `mubra-chemistry-app.html` and locate this section:

```javascript
const CONFIG = {
    GEMINI_API_KEY: 'YOUR_GEMINI_API_KEY_HERE',  // ← Replace with your actual key
    GEMINI_MODEL: 'gemini-1.5-flash',
    GEMINI_API_URL: 'https://generativelanguage.googleapis.com/v1beta/models'
};
```

Replace `'YOUR_GEMINI_API_KEY_HERE'` with your actual API key:

```javascript
const CONFIG = {
    GEMINI_API_KEY: 'AIzaSyD_YourActualKeyHere_AbCdEfGhIjKlMnOp',
    GEMINI_MODEL: 'gemini-1.5-flash',
    GEMINI_API_URL: 'https://generativelanguage.googleapis.com/v1beta/models'
};
```

### Step 3: Test Locally (Optional)

Open `mubra-chemistry-app.html` in your web browser:
- Double-click the file, or
- Right-click → "Open with" → Select your browser

The app will work instantly without any server requirements!

### Step 4: Deploy to GitHub Pages

#### Option A: Deploy Your Entire Repository

1. **Create a GitHub Repository**
   ```bash
   # Initialize git in your project folder
   git init
   git add mubra-chemistry-app.html
   git commit -m "Initial commit: Mubra AI Chemistry App"
   ```

2. **Push to GitHub**
   - Create a new repository on [GitHub.com](https://github.com)
   - Copy the repository URL
   ```bash
   git remote add origin https://github.com/YourUsername/mubra-chemistry.git
   git branch -M main
   git push -u origin main
   ```

3. **Enable GitHub Pages**
   - Go to Repository Settings → **Pages**
   - Source: **Deploy from a branch**
   - Branch: **main**, folder: **/(root)**
   - Click **Save**

4. **Access Your App**
   - Your app will be live at: `https://YourUsername.github.io/mubra-chemistry/mubra-chemistry-app.html`

#### Option B: Single File (Simpler)

1. Rename file to `index.html`
2. Create repository named `YourUsername.github.io`
3. Push `index.html` to the repository
4. Access at: `https://YourUsername.github.io`

---

## 📖 User Guide

### 🧭 Navigation

**Left Sidebar:**
- **📚 පාඩම් (Lessons)**: Select your chapter
  - ⚛️ Organic Chemistry
  - 🔬 Inorganic Chemistry
  - 📊 Physical Chemistry

- **📋 Past Papers**: Browse by year (1985-2025)
  - Click any year to focus on that paper's questions

**Header:** Shows current lesson/year context

**Chat Window:** Ask your questions, get AI responses with:
- Step-by-step explanations
- Chemical formulas rendered beautifully
- Sinhala language answers

### 💬 How to Ask Questions

**Good questions:**
- "Explain the mechanism of the SN2 reaction with an example"
- "What is the hybridisation of carbon in benzene?"
- "2015 paper, question 5: How would you distinguish between primary and secondary alcohols?"
- "Calculate Kp for the reaction: 2SO2(g) + O2(g) ⇌ 2SO3(g) at 500K"

**The AI will:**
- Provide detailed step-by-step explanations
- Use proper chemistry notation
- Reference past papers when relevant
- Explain marking scheme logic
- Give encouraging guidance

---

## 🎨 Design Architecture

### Visual Identity

| Element | Color | Usage |
|---------|-------|-------|
| Primary Navy | #001F3F | Main background, user bubbles |
| Light Navy | #003366 | Hover states, gradients |
| Gold | #D4AF37 | Accents, AI bubbles, borders |
| Gold Light | #E8C547 | Text highlights |
| Background | #f8f8f8 | Main content area |

### Typography

- **Display Font**: Cormorant Garamond (elegant, serif)
  - Logo, headers, titles
- **Body Font**: Lato (clean, readable)
  - Content, messages, UI text

### Layout

```
┌─────────────────────────────────────────────────┐
│                    HEADER                        │
├──────────────┬────────────────────────────────────┤
│              │                                    │
│  SIDEBAR     │         CHAT CONTAINER             │
│  (280px)     │         (scrollable)               │
│              │                                    │
│  • Lessons   │  • Welcome or Messages             │
│  • Years     │  • User: Navy Blue                 │
│  • Links     │  • AI: White + Gold Border        │
│              │                                    │
├──────────────┴────────────────────────────────────┤
│           INPUT AREA (User Input Box)            │
└────────────────────────────────────────────────────┘
```

### Responsive Behavior

- **Desktop (1024px+)**: Full layout with 280px sidebar
- **Tablet (768-1023px)**: Adjusted spacing, responsive chat bubbles
- **Mobile (480-767px)**: Horizontal sidebar, optimized touch targets
- **Small Phone (<480px)**: Stack layout, minimal padding

---

## 🔧 Technical Details

### Technology Stack

| Technology | Purpose |
|-----------|---------|
| **HTML5** | Semantic structure |
| **CSS3** | Styling, animations, gradients, responsive design |
| **Vanilla JavaScript** | All interactivity (no frameworks) |
| **Google Gemini API** | AI responses |
| **KaTeX** | Chemistry formula rendering |
| **CDN Hosted** | No build process, instant deployment |

### Key Implementation Details

#### System Instruction (Sinhala Prompt)
```
ඔබ "Mubra AI 8.v1" නම් විසිඳුම්ශීලී ශ්‍රී ලංකා රසායන විද්‍යා ගුරුවරයි.
(Translation: "You are Mubra AI 8.v1, a legendary Sri Lankan Chemistry expert...")
```

The system prompt ensures:
- Sinhala-only responses
- Deep knowledge of A/L syllabus
- Step-by-step explanations
- Past paper awareness (1985-2025)

#### API Integration

```javascript
// Minimal API setup
const response = await fetch(
    `${GEMINI_API_URL}/${GEMINI_MODEL}:generateContent?key=${API_KEY}`,
    {
        method: 'POST',
        headers: { 'Content-Type': 'application/json' },
        body: JSON.stringify(requestBody)
    }
);
```

#### KaTeX Rendering

```javascript
renderMathInElement(element, {
    delimiters: [
        { left: '$$', right: '$$', display: true },
        { left: '$', right: '$', display: false }
    ]
});
```

Chemistry formulas render automatically in AI responses!

---

## 🔒 Security & Privacy

### Important Notes

⚠️ **API Key Security**:
- Your API key is stored in the HTML file
- For production: Consider using a backend server to hide the API key
- GitHub pages deployment: Anyone can see your key in the source code
- Use GitHub Secrets or environment variables for serious projects

### Recommendations

1. **For Learning**: Current setup is fine (use free tier API key)
2. **For Production**: 
   - Deploy a backend server (Node.js, Python, etc.)
   - Store API key as environment variable
   - Authenticate users
   - Rate limit requests

---

## 📊 API Usage & Costs

### Google Gemini API Pricing (as of 2025)

| Model | Input | Output | Daily Limit |
|-------|-------|--------|------------|
| gemini-1.5-flash | Free | Free | 15,000 requests |
| gemini-1.5-pro | $3.50/M tokens | $10.50/M tokens | - |

**Free Tier Benefits:**
- 15,000 free requests per day
- Perfect for learning
- No credit card required initially

**To upgrade:**
1. Add a payment method in Google Cloud Console
2. Increase daily limits
3. Access premium models

---

## 🐛 Troubleshooting

### Issue: "API Key is not valid"
**Solution:** 
- Verify your key is correctly copied in CONFIG
- Check key has no extra spaces
- Regenerate key in Google AI Studio

### Issue: "No response from AI"
**Solution:**
- Check internet connection
- Verify API key is active
- Check daily request limit (15,000 free limit)
- Open browser DevTools (F12) → Console for error messages

### Issue: "Chemistry formulas not rendering"
**Solution:**
- KaTeX loads from CDN, ensure internet connection
- Check browser console for loading errors
- Refresh the page

### Issue: "Sinhala text showing incorrectly"
**Solution:**
- Ensure page is saved as UTF-8
- Check `<meta charset="UTF-8">` in HTML head
- Update your browser

---

## 📚 Example Conversations

### Example 1: Organic Chemistry Mechanism
```
User: Explain the mechanism of the SN2 reaction with propyl chloride and sodium hydroxide

Mubra AI: දිගු පිළිතුරු...
[Detailed mechanism in Sinhala with chemical formulas and step-by-step progression]
```

### Example 2: Past Paper Question
```
User: 2020 past paper, question 3: How would you prepare ethanoic acid in the laboratory?

Mubra AI: ඔබ 2020 කඩදාසි ගිණුම් කිරීමට අසයි...
[Comprehensive answer with reagents, conditions, mechanism, and safety notes]
```

### Example 3: Calculation
```
User: Calculate Kp for the reaction: N2 + 3H2 ⇌ 2NH3 at 500K

Mubra AI: කරුණාකර පිළිතුරු...
[Step-by-step calculation with formula derivation and numerical result]
```

---

## 🎓 Educational Use Cases

**For Students:**
- 📖 Study difficult topics with personalized explanations
- 📋 Practice past papers with detailed solutions
- 🧪 Understand reaction mechanisms visually
- 🔢 Get help with stoichiometry calculations
- ✍️ Perfect your exam answers

**For Teachers:**
- 📊 Show rich explanations in class
- 🧠 Supplement traditional teaching
- 📚 Access historical exam trends (1985-2025)
- 🎯 Provide students with 24/7 support tool

---

## 🌟 Advanced Customization

### Change Color Scheme

Modify CSS variables in the `<style>` section:

```css
:root {
    --navy-primary: #001F3F;      /* Change primary color */
    --gold-primary: #D4AF37;       /* Change accent color */
    --bg-light: #f8f8f8;           /* Change background */
}
```

### Change AI Personality

Modify `SYSTEM_INSTRUCTION` variable:

```javascript
const SYSTEM_INSTRUCTION = `
ඔබ "Mubra AI 8.v1" නම්...
[Edit the Sinhala prompt here]
`;
```

### Add More Lessons

Add new sidebar items:

```html
<div class="sidebar-item" data-lesson="analytical">
    <span>🔍</span> Analytical Chemistry
</div>
```

---

## 📝 File Structure

```
mubra-chemistry-app.html    (Single file - everything included!)
├── HTML5 Structure
├── CSS3 Styling (embedded)
├── Vanilla JavaScript (embedded)
├── External CDN Links
│   ├── Google Fonts
│   ├── KaTeX Math Rendering
│   └── Google Gemini API
```

**Why single file?**
- ✅ Easy to deploy
- ✅ No build process needed
- ✅ Works offline (with API key)
- ✅ Perfect for GitHub Pages
- ✅ Simple to customize

---

## 🚀 Deployment Checklist

- [ ] Get Google Gemini API key
- [ ] Replace API key in CONFIG
- [ ] Test locally in browser
- [ ] Create GitHub repository
- [ ] Push HTML file to GitHub
- [ ] Enable GitHub Pages in Settings
- [ ] Verify app is live
- [ ] Share link with students!

---

## 📞 Support & Resources

### Learning Resources
- [Google Gemini API Docs](https://ai.google.dev)
- [KaTeX Documentation](https://katex.org)
- [MDN Web Docs](https://developer.mozilla.org)
- [GitHub Pages Guide](https://pages.github.com)

### Sri Lankan A/L Chemistry
- Department of Examinations (SL)
- G.C.E. A/L Curriculum Guides
- Past Paper Archives (1985-2025)

---

## 📄 License

This project is provided as-is for educational purposes.

---

## 🙏 Credits

**Mubra AI 8.v1** - Premium AI Chemistry Tutor  
Built for Sri Lankan G.C.E. A/L Students  
Engineered for Excellence  

---

## 🎯 Future Enhancements

Potential features:
- 📊 Interactive molecular 3D visualization
- 📝 Notes & bookmarks system
- 📈 Progress tracking
- 🎯 Topic-wise quiz mode
- 📱 Native mobile app
- 🗣️ Voice input/output
- 🌙 Dark mode toggle
- 🔐 User authentication

---

**Made with ❤️ for Sri Lankan Chemistry Students**  
_Engineered for Excellence_

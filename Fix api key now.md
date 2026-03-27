# 🔑 API Key Issue - Fix කරන්න!

## 🔴 **Problem**

ඔබගේ code එකෙන් දිස්වෙනවා:

```javascript
if (CONFIG.GEMINI_API_KEY === 'AIzaSyAZBSRcSLLEwY-UbsghSnCZoQA7CJNRa4') {
```

**ඔබ placeholder එක replace කර නැත!** 😅

---

## ✅ **Fix කරන්න - 2 Steps**

### **Step 1: Google එකින් API Key ගන්න**

```
1. https://aistudio.google.com ට යන්න
2. "Get API key" click කරන්න
3. "Create API key in new project" click
4. API key copy කරන්න (දිස්වෙන text එක)

Looks like: AIzaSyD_XXXXXXXX-XXXXXXXX-XXXXXXXX_XXXXXXXX
```

### **Step 2: HTML File එක Update කරන්න**

**mubra-chemistry-app.html open කරන්න** (text editor)

**Ctrl+F press කරන්න** (Find)

**Search කරන්න:** `PASTE_YOUR_API_KEY_HERE`

**Find කරපු part:**
```javascript
const CONFIG = {
    GEMINI_API_KEY: 'PASTE_YOUR_API_KEY_HERE',
    GEMINI_MODEL: 'gemini-1.5-flash',
    GEMINI_API_URL: 'https://generativelanguage.googleapis.com/v1beta/models'
};
```

**Replace කරන්න:**
```javascript
const CONFIG = {
    GEMINI_API_KEY: 'AIzaSyD_YOUR_REAL_KEY_HERE',  // ← Your Google API key
    GEMINI_MODEL: 'gemini-1.5-flash',
    GEMINI_API_URL: 'https://generativelanguage.googleapis.com/v1beta/models'
};
```

**උදාහරණ:**
```javascript
// If your key is: AIzaSyABC123def456ghi789
// Then put:
GEMINI_API_KEY: 'AIzaSyABC123def456ghi789',
```

---

## 📝 **Complete Example**

**BEFORE:**
```javascript
const CONFIG = {
    GEMINI_API_KEY: 'PASTE_YOUR_API_KEY_HERE',
    GEMINI_MODEL: 'gemini-1.5-flash',
    GEMINI_API_URL: 'https://generativelanguage.googleapis.com/v1beta/models'
};
```

**AFTER (with real key):**
```javascript
const CONFIG = {
    GEMINI_API_KEY: 'AIzaSyD_12345-67890-ABCDE-FGHIJ',
    GEMINI_MODEL: 'gemini-1.5-flash',
    GEMINI_API_URL: 'https://generativelanguage.googleapis.com/v1beta/models'
};
```

---

## 💾 **Save & Test**

```
1. Ctrl+S (Windows) හෝ Cmd+S (Mac)
2. File එක save වෙලා!

3. Double-click: mubra-chemistry-app.html
4. Browser open වෙනවා
5. Chat window දිස්වෙනවා
6. Type: "What is chemistry?"
7. Send (📤)
8. ✅ AI response එක දිස්වෙනවා!
```

---

## ✨ **දැන් ඉතිරි කරන්න:**

```
const CONFIG = {
    GEMINI_API_KEY: 'YOUR_REAL_KEY_HERE',
    GEMINI_MODEL: 'gemini-1.5-flash',
    GEMINI_API_URL: 'https://generativelanguage.googleapis.com/v1beta/models'
};
```

---

## 🚨 **IMPORTANT - Again!**

```
⚠️ API Key එක කිසිවෙක්ටු share කරන්ට එපා!
✅ Keep PRIVATE
✅ Local computer එකට විතරක්
✅ Password manager එකට save කරන්න
✅ Never GitHub public repo එකට commit කරන්ට එපා
```

---

## 🤔 **still error ඉතින්?**

```
1. API key correct copy කරපු නම් check කරන්න
2. Extra spaces නැති බව බලන්න
3. Single quotes 'xxx' තුල තිබුණේ නම් check කරන්න
4. Save කරපු නම් check කරන්න

New API key දිගින් නැවත උත්සහ කරන්න!
```

---

**Ready now?** 🚀

1. Google API key ගන්න
2. HTML file update කරන්න
3. Save කරන්න
4. Test කරන්න!

**Success! 🎉**

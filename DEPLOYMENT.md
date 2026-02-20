# 🚀 GitHub Pages Deployment Guide

## ✅ What's Been Fixed

### 1. File Organization
- ✅ Created `index.html` in root directory
- ✅ Renamed resume to `resume.pdf`
- ✅ Created `/images` folder for all images
- ✅ Created `/certificates` folder for certificates
- ✅ Removed spaces and special characters from filenames

### 2. Updated Paths
- ✅ Resume link: `href="resume.pdf"`
- ✅ All image paths: `images/filename.jpg` (relative, no leading slash)
- ✅ Education images: `images/srm-university.png`, `images/mohamed-sathak-college.png`
- ✅ Internship image: `images/hepl-logo.png`
- ✅ Project images: `images/ckd-project.jpg`, `images/bill-management.jpg`, `images/hm-logo.png`

### 3. External Links
- ✅ Social links open in new tab with `target="_blank" rel="noopener noreferrer"`
- ⚠️ Update LinkedIn and GitHub URLs in footer (currently placeholder)

## 📋 Before You Deploy

### Update Your Social Links
Open `index.html` and find the footer section. Update these lines:

```html
<!-- Find and replace with your actual URLs -->
<a href="https://www.linkedin.com/in/YOUR-LINKEDIN-USERNAME" class="social-link" target="_blank" rel="noopener noreferrer">
<a href="https://github.com/YOUR-GITHUB-USERNAME" class="social-link" target="_blank" rel="noopener noreferrer">
```

## 🌐 Deploy to GitHub Pages

### Option 1: Using Git Commands

```bash
# Navigate to your portfolio folder
cd c:\Users\yousuf\OneDrive\Desktop\GitHub\yousufportfolio

# Initialize git repository
git init

# Add all files
git add .

# Commit
git commit -m "Deploy portfolio to GitHub Pages"

# Create main branch
git branch -M main

# Add remote (replace YOUR-USERNAME with your GitHub username)
git remote add origin https://github.com/YOUR-USERNAME/yousufportfolio.git

# Push to GitHub
git push -u origin main
```

### Option 2: Using GitHub Desktop

1. Open GitHub Desktop
2. File → Add Local Repository
3. Choose: `c:\Users\yousuf\OneDrive\Desktop\GitHub\yousufportfolio`
4. Click "Publish repository"
5. Uncheck "Keep this code private" if you want it public
6. Click "Publish Repository"

### Enable GitHub Pages

1. Go to: `https://github.com/YOUR-USERNAME/yousufportfolio`
2. Click **Settings** tab
3. Scroll to **Pages** section (left sidebar)
4. Under **Source**:
   - Branch: `main`
   - Folder: `/ (root)`
5. Click **Save**
6. Wait 2-3 minutes
7. Your site will be live at: `https://YOUR-USERNAME.github.io/yousufportfolio/`

## 🧪 Test Locally Before Deploying

Open `index.html` in your browser and verify:
- [ ] Resume downloads correctly
- [ ] All images load
- [ ] Navigation works
- [ ] Mobile menu works
- [ ] All sections display properly
- [ ] Animations work
- [ ] Social links open in new tab

## 📁 Final File Structure

```
yousufportfolio/
├── index.html                    ← Main file (GitHub Pages looks for this)
├── resume.pdf                    ← Your resume
├── images/                       ← All images
│   ├── srm-university.png
│   ├── mohamed-sathak-college.png
│   ├── hepl-logo.png
│   ├── ckd-project.jpg
│   ├── bill-management.jpg
│   └── hm-logo.png
├── certificates/                 ← For future certificates
├── .gitignore                    ← Excludes unnecessary files
└── README.md                     ← Documentation
```

## ⚠️ Files to Delete (Optional)

These files are not needed for deployment:
- `day4portfolio.html` (old version)
- `yousuf.html` (old version)
- `portfolio.css` (if not used)
- `images.png` (if not used)
- `Sheik_Yousuf_-_new_Resume_2025.pdf_(1)[1].pdf` (old resume)

They're already in `.gitignore` so they won't be pushed to GitHub.

## 🎉 After Deployment

1. Visit your live site
2. Test on mobile devices
3. Share your portfolio link:
   - LinkedIn profile
   - Resume
   - Email signature
   - GitHub profile README

## 🔧 Troubleshooting

### Images not loading?
- Check paths are relative: `images/filename.jpg` (no leading `/`)
- Verify files exist in `/images` folder
- Check filename spelling matches exactly

### Resume not downloading?
- Verify `resume.pdf` exists in root directory
- Check link: `<a href="resume.pdf" download>`

### Page not found (404)?
- Wait 5 minutes after enabling GitHub Pages
- Check repository is public
- Verify `index.html` is in root directory

### Animations not working?
- Check AOS library is loaded: `<script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>`
- Verify AOS.init() is called in JavaScript

## 📞 Need Help?

If you encounter issues:
1. Check browser console for errors (F12)
2. Verify all file paths are correct
3. Test locally first before deploying
4. Check GitHub Pages build status in repository settings

---

✅ Your portfolio is now ready for GitHub Pages deployment!

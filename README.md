# Filecoin Business Plan Calculator - GitHub Pages Setup

This is a standalone HTML file that runs your Filecoin business plan calculator. It's ready to be hosted on GitHub Pages!

## 🚀 Quick Setup Instructions

### Step 1: Create a New GitHub Repository

1. Go to [GitHub](https://github.com) and sign in
2. Click the **+** icon in the top right and select **New repository**
3. Name your repository (e.g., `filecoin-business-plan`)
4. Choose **Public** (required for free GitHub Pages)
5. Click **Create repository**

### Step 2: Upload Your File

**Option A: Using GitHub Web Interface (Easiest)**

1. In your new repository, click **Add file** → **Upload files**
2. Drag and drop the `index.html` file
3. Add a commit message like "Initial commit"
4. Click **Commit changes**

**Option B: Using Git Command Line**

```bash
# Navigate to where you saved index.html
cd /path/to/your/file

# Initialize git repository
git init

# Add your file
git add index.html

# Commit
git commit -m "Initial commit: Filecoin business plan calculator"

# Add your GitHub repository as remote (replace USERNAME and REPO)
git remote add origin https://github.com/USERNAME/REPO.git

# Push to GitHub
git branch -M main
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** (top menu)
3. Click **Pages** in the left sidebar
4. Under **Source**, select **main** branch
5. Click **Save**
6. Wait a minute or two for deployment

### Step 4: Access Your Site

Your site will be available at:
```
https://USERNAME.github.io/REPO/
```

For example, if your username is `johndoe` and your repo is `filecoin-business-plan`:
```
https://johndoe.github.io/filecoin-business-plan/
```

## 📝 What's Included

The `index.html` file contains:
- ✅ Complete React application (no build step needed!)
- ✅ Recharts for interactive charts
- ✅ Tailwind CSS for styling
- ✅ All loaded from CDN - no dependencies to install
- ✅ Interactive inputs to adjust calculations
- ✅ Financial projections and visualizations

## 🎨 Customization

You can customize the calculator by editing the `index.html` file:

- **Default values**: Lines 7-9 contain the initial storage capacity, power cost, and datacap multiplier
- **Financial assumptions**: Lines 10-21 contain hardware costs, financing terms, etc.
- **Operational costs**: Lines 23-36 contain monthly operating expenses
- **Revenue model**: Lines 42-50 contain FIL pricing and reward rates

## 🔄 Updating Your Site

Whenever you want to make changes:

1. Edit `index.html` locally
2. Upload the new version to GitHub (or commit and push via git)
3. GitHub Pages will automatically rebuild (takes 1-2 minutes)

## 💡 Tips

- The calculator works entirely in the browser - no backend needed
- All calculations happen in real-time as users adjust the inputs
- The site is responsive and works on mobile devices
- You can share the URL with investors, partners, or team members

## 🐛 Troubleshooting

**Site not showing up?**
- Wait 2-3 minutes after enabling GitHub Pages
- Check that your repository is Public
- Verify the file is named exactly `index.html`

**Charts not displaying?**
- Open browser console (F12) to check for errors
- Ensure you have a stable internet connection (CDN libraries need to load)

**Need help?**
- Check GitHub Pages documentation: https://pages.github.com/
- Verify your repository settings under Settings → Pages

---

**Created with Claude** 🤖

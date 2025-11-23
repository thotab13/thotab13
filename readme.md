# 📝 How to Set Up Your GitHub Profile README

## Step 1: Create a Special Repository

1. **Go to GitHub** and click the **"+"** icon in the top right corner
2. Click **"New repository"**
3. **IMPORTANT**: Name the repository **exactly** as your GitHub username
   - For example, if your username is `thotab13`, name the repository `thotab13`
4. ✅ Check the box **"Add a README file"**
5. Select **"Public"** (must be public to show on your profile)
6. Click **"Create repository"**

🎉 GitHub will show a special message: *"You found a secret! thotab13/thotab13 is a ✨special✨ repository"*

---

## Step 2: Edit the README File

### Option A: Edit Directly on GitHub (Easiest)

1. In your new repository, click on the **`README.md`** file
2. Click the **pencil icon** (✏️) that says "Edit this file"
3. **Delete all existing content** in the file
4. **Copy the entire README** I created for you (from the artifact above)
5. **Paste it** into the editor
6. Scroll down and click **"Commit changes"**
7. Add a commit message like "Update profile README"
8. Click **"Commit changes"** again

### Option B: Edit Using GitHub Desktop (Alternative)

1. Open **GitHub Desktop**
2. Click **"File"** → **"Clone repository"**
3. Select your `thotab13` repository and clone it
4. Open the **README.md** file in a text editor (VS Code, Notepad++, etc.)
5. Replace all content with the new README
6. Save the file
7. Go back to GitHub Desktop
8. Write a commit message like "Update profile README"
9. Click **"Commit to main"**
10. Click **"Push origin"**

### Option C: Using Git Command Line

```bash
# Clone your repository
git clone https://github.com/thotab13/thotab13.git
cd thotab13

# Edit README.md with your favorite editor
nano README.md  # or use: code README.md, vim README.md, etc.

# Save and commit
git add README.md
git commit -m "Update profile README"
git push origin main
```

---

## Step 3: Customize Your README

### Update These Sections:

#### 1. **GitHub Username**
Replace `thotab13` with your actual username in:
- `https://github-readme-stats.vercel.app/api?username=thotab13`
- `https://github-readme-streak-stats.herokuapp.com/?user=thotab13`
- `https://github-readme-stats.vercel.app/api/top-langs/?username=thotab13`
- `https://github-profile-trophy.vercel.app/?username=thotab13`
- Snake game path (if you add it)

#### 2. **Social Links**
Update these URLs:
```markdown
<a href='https://www.linkedin.com/in/bhuvan'>
<a href='https://github.com/thotab13'>
<a href='https://bhuvana-chandra-portfolio.com'>
```

#### 3. **Contact Information**
The template uses your resume info, but you can customize:
- Phone number (if you want to add it)
- Email
- Location

#### 4. **Cover Image** (Optional)
Change the header image by replacing this URL:
```markdown
<img width="100%" height = "250px" src="https://cdn.pixabay.com/photo/2018/01/14/23/12/nature-3082832_1280.jpg" alt="cover" />
```

Find free images at:
- [Unsplash](https://unsplash.com)
- [Pixabay](https://pixabay.com)
- [Pexels](https://pexels.com)

---

## Step 4: View Your Profile

1. Go to **your GitHub profile**: `https://github.com/thotab13`
2. Your README will now appear at the top of your profile! 🎉
3. It may take a few seconds to update

---

## 🎨 Optional Enhancements

### Add a Snake Animation (Cool Feature!)

1. Create a new file in your repository: `.github/workflows/snake.yml`
2. Add this code:

```yaml
name: Generate Snake

on:
  schedule:
    - cron: "0 */12 * * *"
  workflow_dispatch:

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v2
      - uses: Platane/snk@master
        with:
          github_user_name: thotab13
          outputs: |
            dist/github-contribution-grid-snake.svg
            dist/github-contribution-grid-snake-dark.svg?palette=github-dark
      - uses: crazy-max/ghaction-github-pages@v2.1.3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

3. Commit the file
4. Go to **Actions** tab and enable workflows
5. Run the workflow manually first

### Add Visitor Counter

Add this to your README:
```markdown
![Visitor Count](https://profile-counter.glitch.me/thotab13/count.svg)
```

---

## 📋 Quick Checklist

- [ ] Created repository with your exact username
- [ ] Repository is set to **Public**
- [ ] Copied and pasted the README content
- [ ] Updated GitHub username in all stats sections
- [ ] Updated LinkedIn and portfolio links
- [ ] Committed changes
- [ ] Checked your profile to see the changes

---

## 🔧 Troubleshooting

**Q: My README isn't showing up**
- Make sure the repository name matches your username exactly
- Make sure the repository is public
- Wait a few minutes and refresh

**Q: Images/badges aren't loading**
- Check your internet connection
- The external services might be temporarily down
- Try refreshing after a few minutes

**Q: Stats cards show "username not found"**
- Make sure you replaced `thotab13` with YOUR username
- Check that your username is spelled correctly

**Q: How do I make changes later?**
- Just edit the README.md file again following Step 2
- Changes appear instantly after committing

---

## 📚 Useful Resources

- [GitHub Profile README Guide](https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-github-profile/customizing-your-profile/managing-your-profile-readme)
- [Awesome GitHub Profile README](https://github.com/abhisheknaiidu/awesome-github-profile-readme)
- [GitHub Readme Stats](https://github.com/anuraghazra/github-readme-stats)
- [Shields.io](https://shields.io/) - For custom badges

---

**Need help?** Feel free to ask me any questions! 🚀

# GitHub Profile Setup Instructions

## What This Is
This is a **special GitHub repository** that will display on your profile page at `github.com/MatthewJamisonJS`. When you create a repository with the same name as your username (`MatthewJamisonJS`), GitHub automatically shows its README on your profile.

## Files in This Directory
- `README.md` - Your profile content (narrative, badges, links)
- `coding.gif` - Your animated coding video (9.4MB, optimized)
- `coding.mp4` - Original video (backup, optional to commit)
- `SETUP.md` - These instructions

## Setup Steps

### 1. Initialize Git Repository (using jj)
```bash
cd MatthewJamisonJS
jj git init --git-repo .
```

### 2. Create the GitHub Repository
Go to https://github.com/new and create a new repository:
- Repository name: `MatthewJamisonJS` (MUST match your username exactly)
- Description: "My GitHub profile README"
- Visibility: **Public** (required for profile READMEs)
- **DO NOT** initialize with README, .gitignore, or license (we already have files)

### 3. Add Files and Push
```bash
# Stage all files
jj git add README.md coding.gif

# Optional: Add the MP4 if you want backup (adds ~1.2MB)
# jj git add coding.mp4

# Create first commit
jj commit -m "Add profile README with animated banner"

# Set remote (replace with your actual repo URL)
jj git remote add origin git@github.com:MatthewJamisonJS/MatthewJamisonJS.git

# Push to GitHub
jj git push --set-upstream origin main
```

### 4. Verify Your Profile
Visit `https://github.com/MatthewJamisonJS` to see your new profile README!

## Customization Ideas
- Update the "Recent Highlights" section with new accomplishments
- Add more tech badges from https://shields.io/
- Update anime references as you watch new shows
- Add a "Currently Learning" section for new technologies
- Include a GitHub stats widget: https://github.com/anuraghazra/github-readme-stats

## Troubleshooting

**GIF not showing?**
- Make sure the file is committed and pushed
- Check file size is under 25MB (yours is 9.4MB ✅)
- Verify the image path in README.md matches the filename

**Profile not updating?**
- Repository must be named exactly `MatthewJamisonJS`
- Repository must be public
- Give it a few minutes for GitHub to update the cache

**Want to change the animation?**
- Replace `coding.gif` with a new image/GIF
- Keep dimensions around 600px wide for consistency
- Commit and push the changes

## Need Help?
Reach out if you need any adjustments to the narrative, badges, or layout!

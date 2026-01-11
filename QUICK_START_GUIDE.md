# Quick Start Guide - Week 1 GitHub Setup

## Step-by-Step Instructions for Uploading to GitHub

### Prerequisites
- GitHub account created
- Git installed on your computer
- All Week 1 files downloaded from this package

---

## Option 1: Using GitHub Web Interface (Easiest for Beginners)

### Step 1: Create Repository on GitHub
1. Go to [github.com](https://github.com) and log in
2. Click the "+" icon in top right → "New repository"
3. Fill in details:
   - Repository name: `capstone-part-b` (or your preferred name)
   - Description: "Capstone Part B Project Repository"
   - Make it **Private** (recommended for academic work)
   - ✅ Check "Add a README file"
   - ✅ Add .gitignore: Select "None" (we'll add our own)
4. Click "Create repository"

### Step 2: Upload Files via Web Interface
1. In your new repository, click "Add file" → "Upload files"
2. Drag and drop ALL the files from this package:
   - README.md
   - .gitignore
   - docs/ folder (with all subfolders)
   - evidence/ folder (with all subfolders)
   - research/ folder
   - analysis/ folder
   - framework/ folder
3. In the commit message box at bottom, write:
   ```
   [WEEK-1] Initial repository setup with folder structure and documentation
   ```
4. Click "Commit changes"

### Step 3: Add Evidence Files
1. Navigate to `evidence/week-1/` folder in your repository
2. Click "Add file" → "Upload files"
3. Upload your evidence items:
   - E1_kickoff_meeting_minutes.pdf
   - E2_system_specification_v1.1.docx
   - E3_mvp_confirmation.docx
   - E4_github_screenshots.pdf
   - E5_ethics_considerations.docx
4. Commit message: `[WEEK-1] Add Week 1 evidence items E1-E5`
5. Click "Commit changes"

### Step 4: Verify Your Repository
Check that you have:
- [ ] All folders visible (docs, evidence, research, analysis, framework)
- [ ] README.md file displaying on main page
- [ ] Project logs in docs/project-logs/
- [ ] Meeting minutes in docs/meeting-minutes/
- [ ] Evidence files in evidence/week-1/
- [ ] At least 2-3 commits showing in commit history

---

## Option 2: Using Git Command Line (Recommended)

### Step 1: Create Repository on GitHub
Same as Option 1, Step 1 above.

### Step 2: Clone Repository to Your Computer
```bash
# Open Terminal (Mac/Linux) or Git Bash (Windows)
cd ~/Documents  # or wherever you want the project

# Clone your repository (replace with your URL)
git clone https://github.com/YOUR-USERNAME/capstone-part-b.git
cd capstone-part-b
```

### Step 3: Add All Files
```bash
# Copy all files from this package into the cloned folder
# Then add them to Git:

git add .
git commit -m "[WEEK-1] Initial repository setup with folder structure and documentation"
git push origin main
```

### Step 4: Add Evidence Files
```bash
# Copy your evidence files to evidence/week-1/
# Then:

git add evidence/week-1/
git commit -m "[WEEK-1] Add Week 1 evidence items E1-E5"
git push origin main
```

### Step 5: Verify on GitHub
Open your repository in a web browser and verify all files are there.

---

## What to Do With Each File in This Package

| File/Folder | Action Required | Description |
|-------------|----------------|-------------|
| **README.md** | ✏️ Edit then upload | Update with your name, project title, supervisor |
| **.gitignore** | ✅ Upload as-is | Prevents committing unnecessary files |
| **docs/GIT_GUIDE.md** | ✅ Upload as-is | Reference guide for Git usage |
| **docs/project-logs/** | ✏️ Edit then upload | Fill in your project details in Week_1_Project_Log.docx |
| **docs/meeting-minutes/** | ✏️ Edit then upload | Fill in your meeting details in Week_1_Meeting_Minutes.docx |
| **evidence/README.md** | ✅ Upload as-is | Guide for organizing evidence |
| **evidence/week-1/** | 📤 Add your files | Upload YOUR evidence items (E1-E5) |
| **research/** | 📂 Keep for later | Use in Week 2+ for literature review |
| **analysis/** | 📂 Keep for later | Use in Week 2+ for case studies |
| **framework/** | 📂 Keep for later | Use in Week 2+ for framework development |

---

## Evidence Items You Need to Create for Week 1

You need to create and upload these 5 evidence items:

### E1: Kickoff Meeting Minutes
- **What**: PDF or DOCX of your actual meeting minutes
- **Template**: Use the `Week_1_Meeting_Minutes.docx` as a starting point
- **Where**: Save as `E1_kickoff_meeting_minutes.pdf` in `evidence/week-1/`

### E2: System Specification v1.1
- **What**: Your updated system specification from Part A
- **Where**: Save as `E2_system_specification_v1.1.docx` in `evidence/week-1/`

### E3: MVP Confirmation
- **What**: Document defining your Minimum Viable Product
- **Where**: Save as `E3_mvp_confirmation.docx` in `evidence/week-1/`

### E4: GitHub Setup Screenshots
- **What**: Screenshots showing:
  - Repository folder structure
  - Commit history with meaningful messages (minimum 3 commits)
  - README file
- **Where**: Combine into `E4_github_screenshots.pdf` in `evidence/week-1/`

### E5: Ethics & Considerations
- **What**: Document addressing ethics, security, privacy, sustainability
- **Where**: Save as `E5_ethics_considerations.docx` in `evidence/week-1/`

---

## Filling Out the Templates

### Week 1 Project Log (docs/project-logs/Week_1_Project_Log.docx)

Replace all `[placeholders]` with your actual information:

1. **Project Information Table**:
   - Your name(s)
   - Student ID(s)
   - Project title
   - Supervisor name
   - GitHub URL

2. **Section 1 - Summary**: Describe what you actually accomplished in Week 1

3. **Section 2 - Evidence**: Reference your evidence items (E1-E5)

4. **Section 3 - Environment Setup**: Describe your actual setup

5. **Section 4 - Specification Refinement**: Detail your scope and requirements

6. **Section 5 - Risks**: List your actual risks and mitigation strategies

7. **Section 6 - Next Week Plan**: What you'll do in Week 2

### Week 1 Meeting Minutes (docs/meeting-minutes/Week_1_Meeting_Minutes.docx)

Fill in:
1. Meeting date, time, location
2. Attendees
3. Decisions made
4. Risks identified
5. Action items with owners and due dates

---

## Checklist Before Submission

Use this checklist to ensure everything is ready:

### GitHub Repository Setup
- [ ] Repository created on GitHub
- [ ] Repository is private (recommended)
- [ ] README.md uploaded and customized with your details
- [ ] .gitignore file uploaded
- [ ] Folder structure created (docs, evidence, research, analysis, framework)

### Documentation
- [ ] Week_1_Project_Log.docx completed and uploaded
- [ ] Week_1_Meeting_Minutes.docx completed and uploaded
- [ ] All placeholders replaced with actual information
- [ ] Documents professionally formatted

### Evidence Items
- [ ] E1: Kickoff meeting minutes uploaded
- [ ] E2: System specification v1.1 uploaded
- [ ] E3: MVP confirmation uploaded
- [ ] E4: GitHub screenshots uploaded
- [ ] E5: Ethics considerations uploaded
- [ ] All evidence files properly named

### Git Commits
- [ ] At least 3 meaningful commits
- [ ] Commit messages follow [WEEK-1] format
- [ ] Commits show incremental progress
- [ ] All files pushed to GitHub

### Quality Check
- [ ] All evidence is clearly labeled and referenced in Project Log
- [ ] Screenshots are clear and readable
- [ ] Documents have no spelling/grammar errors
- [ ] Repository is organized and professional
- [ ] Can access everything via GitHub web interface

---

## Common Issues and Solutions

### Issue: "Repository not found" error
**Solution**: Make sure you've created the repository on GitHub first.

### Issue: Files not showing up after commit
**Solution**: Run `git push origin main` to push changes to GitHub.

### Issue: Large files won't upload
**Solution**: 
- GitHub has a 100MB file size limit
- Compress large files or use Git LFS for files >50MB
- Consider splitting large evidence into multiple files

### Issue: Can't edit .docx files on GitHub
**Solution**: 
- Download the file, edit locally, then re-upload
- Or use Git command line to update files

### Issue: Forgot to commit something
**Solution**:
```bash
git add forgotten-file.txt
git commit -m "[WEEK-1] Add forgotten file"
git push origin main
```

---

## Getting Repository URL for Your Project Log

After creating your repository:

1. Go to your repository on GitHub
2. Click the green "Code" button
3. Copy the HTTPS URL (e.g., `https://github.com/username/capstone-part-b`)
4. Paste this URL in your Project Log where it asks for "Git Repository URL"

---

## Next Steps After Week 1

1. **Week 2**: Begin literature review and research
2. **Regular commits**: Commit your work at least 2-3 times per week
3. **Evidence tracking**: Keep adding evidence to respective week folders
4. **Meeting minutes**: Continue documenting all meetings
5. **Project logs**: Prepare Week 3 and Week 6 logs following same structure

---

## Need Help?

- **Git Guide**: See `docs/GIT_GUIDE.md` for detailed Git commands
- **Evidence Guide**: See `evidence/README.md` for evidence requirements
- **GitHub Help**: https://docs.github.com/
- **Supervisor**: Contact your supervisor with questions

---

**Remember**: Git usage is mandatory and will be assessed. Make regular commits showing continuous progress!

*Good luck with Week 1! 🚀*

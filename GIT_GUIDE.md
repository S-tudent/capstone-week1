# Git Usage Guide for Capstone Project

## Importance of Git for Assessment

Git usage is **mandatory** and will be reviewed as part of Assessment 1. Your commit history demonstrates:
- Continuous technical progress
- Incremental development practices
- Professional version control habits
- Evidence of implementation work

## Commit Message Format

Use this format for all commits:
```
[WEEK-X] Brief description of changes

Optional: More detailed explanation if needed
- Bullet point 1
- Bullet point 2
```

### Examples of Good Commit Messages:
```
[WEEK-1] Initial repository setup with folder structure

[WEEK-1] Add project kickoff meeting minutes

[WEEK-1] Update system specification v1.0 to v1.1
- Refined scope definition
- Enhanced functional requirements
- Added framework integration details

[WEEK-1] Document MVP confirmation and components

[WEEK-1] Add evidence items E1-E5 to week-1 folder

[WEEK-2] Begin literature review on ransomware prevention

[WEEK-2] Add 10 research sources to bibliography

[WEEK-3] Implement core data pipeline functionality

[WEEK-3] Add unit tests for data transformation module
```

### Examples of Poor Commit Messages (Avoid These):
```
❌ "update"
❌ "fix"
❌ "changes"
❌ "stuff"
❌ "final version"
❌ "asdf"
```

## Commit Frequency

### Recommended Frequency:
- **Minimum**: 3-5 commits per week
- **Ideal**: Daily or after completing each significant task
- **Evidence-driven**: Commit after each evidence item is ready

### What to Commit:
✅ Documentation (meeting minutes, specifications, logs)
✅ Evidence files (screenshots, PDFs, exports)
✅ Code and scripts (even if incomplete)
✅ README updates
✅ Configuration files

### What NOT to Commit:
❌ Sensitive information (passwords, API keys)
❌ Very large binary files (>10MB)
❌ Temporary files (.tmp, .cache)
❌ IDE-specific files (.idea/, .vscode/ - unless team agrees)
❌ Dependencies (node_modules/, venv/)

## Basic Git Workflow

### Initial Setup (Week 1):
```bash
# Create repository on GitHub first, then:
git clone https://github.com/your-username/your-repo.git
cd your-repo

# Create initial structure
mkdir -p docs/project-logs docs/meeting-minutes docs/specifications
mkdir -p research analysis framework evidence/week-{1,3,6}

# Create README
echo "# Capstone Project Part B" > README.md

# First commit
git add .
git commit -m "[WEEK-1] Initial repository setup with folder structure"
git push origin main
```

### Regular Workflow:
```bash
# 1. Check status
git status

# 2. Add files (be specific, don't use 'git add .' blindly)
git add docs/meeting-minutes/Week_1_Meeting_Minutes.docx
git add evidence/week-1/E1_kickoff_meeting.pdf

# 3. Commit with meaningful message
git commit -m "[WEEK-1] Add kickoff meeting minutes and evidence"

# 4. Push to GitHub
git push origin main

# 5. Verify on GitHub
# Open GitHub in browser and check your commits appear
```

## Tips for Assessment Success

### 1. Make Incremental Commits
Show continuous progress, not one huge commit at the end:
```bash
# Good progression:
[WEEK-1] Create initial project structure
[WEEK-1] Add meeting minutes template
[WEEK-1] Complete and upload kickoff meeting minutes
[WEEK-1] Update system specification document
[WEEK-1] Add evidence items E1-E3
```

### 2. Document Your Work
Your commit history tells a story of your implementation:
```bash
[WEEK-2] Begin literature review research
[WEEK-2] Add 5 research papers on ransomware prevention
[WEEK-2] Add 5 more sources on incident response
[WEEK-2] Create literature review summary document
[WEEK-2] Update evidence folder with research notes
```

### 3. Reference Commits in Your Project Log
Example in Project Log:
> "As evidenced in commit abc123f, we implemented the initial data pipeline on January 15th..."

### 4. Keep Your Repository Organized
```
✅ Good structure:
/docs
  /project-logs
    Week_1_Project_Log.docx
  /meeting-minutes
    Week_1_Meeting_Minutes.docx

❌ Poor structure:
document1.docx
finalversion2.docx
copy_of_minutes.pdf
```

## Common Git Commands

### Checking Status:
```bash
git status                    # See what's changed
git log --oneline            # View commit history (compact)
git log                      # View detailed commit history
```

### Managing Files:
```bash
git add file.txt             # Stage specific file
git add docs/                # Stage entire folder
git add .                    # Stage all changes (use carefully!)
git rm file.txt              # Remove file
git mv old.txt new.txt       # Rename file
```

### Viewing Changes:
```bash
git diff                     # See unstaged changes
git diff --staged            # See staged changes
git show abc123              # Show specific commit
```

### Fixing Mistakes:
```bash
# Undo last commit (keep changes)
git reset --soft HEAD~1

# Undo changes to a file
git checkout -- file.txt

# Amend last commit message (only if not pushed)
git commit --amend -m "[WEEK-1] New message"
```

## Git Workflow for Teams

If working in a team:

### 1. Coordinate Before Pushing:
```bash
# Always pull before starting work
git pull origin main

# Make your changes and commit
git add .
git commit -m "[WEEK-2] Your changes"

# Pull again to get latest changes
git pull origin main

# Push your work
git push origin main
```

### 2. Handle Conflicts:
If you get a merge conflict:
```bash
# Git will mark the conflicting file
# Open the file and look for:
<<<<<<< HEAD
Your changes
=======
Their changes
>>>>>>> abc123

# Resolve the conflict by editing the file
# Then:
git add resolved_file.txt
git commit -m "[WEEK-2] Resolve merge conflict in resolved_file.txt"
git push origin main
```

## Assessment Evidence Checklist

Before each submission, verify:

- [ ] Repository has regular commits (not all on one day)
- [ ] Commit messages follow the [WEEK-X] format
- [ ] Each commit has a meaningful description
- [ ] Evidence items are committed and pushed
- [ ] Repository structure is clean and organized
- [ ] No sensitive information committed
- [ ] All team members have contributed (if applicable)
- [ ] Can access repository from GitHub web interface

## Quick Reference Card

| Task | Command |
|------|---------|
| Clone repository | `git clone <url>` |
| Check status | `git status` |
| Stage file | `git add <file>` |
| Commit changes | `git commit -m "message"` |
| Push to GitHub | `git push origin main` |
| Pull from GitHub | `git pull origin main` |
| View history | `git log --oneline` |
| See differences | `git diff` |

## Resources

- [GitHub Guides](https://guides.github.com/)
- [Git Documentation](https://git-scm.com/doc)
- [Atlassian Git Tutorial](https://www.atlassian.com/git/tutorials)

## Getting Help

If you encounter issues:
1. Check `git status` to see what's happening
2. Search for the error message online
3. Ask your supervisor or classmates
4. Use GitHub's issue tracker for team communication

---
*Remember: Good Git practices demonstrate professional development skills and are part of your assessment!*

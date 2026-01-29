# 🔧 Novice Walkthrough: 30 Flagged Improvements

> **Persona**: MBA student, never used terminal, first time building an app
> **Task**: Read Claude Code instructions and flag every confusion point

---

## 🚩 30 Flagged Improvements

### Section: Prerequisites & Setup

| # | Location | Novice Confusion | Improvement |
|:-:|:---------|:-----------------|:------------|
| 1 | "runs in your terminal" | What's a terminal? Where do I find it? | Add: "Terminal is the app called 'Terminal' on Mac (search Spotlight) or 'Command Prompt' on Windows" |
| 2 | "Download from nodejs.org" | Which version? LTS or Current? | Add: "Download the LTS (Long Term Support) version" |
| 3 | `npm install -g @anthropic-ai/claude-code` | What is npm? Why -g? | Add: "npm is Node's package manager (installed with Node.js). The -g means 'global' so you can use it anywhere" |
| 4 | "Verify installation" | What if it says "command not found"? | Add troubleshooting: "If you see 'command not found', close and reopen Terminal, or restart your computer" |
| 5 | API key not mentioned | Claude Code requires an Anthropic API key! | **CRITICAL**: Add section on getting API key from console.anthropic.com |
| 6 | "Install Git from git-scm.com" | Which options during install? | Add: "Use default options during installation" |
| 7 | "type git --version" | How do I "type" in terminal? | Add screenshot or: "Open Terminal, type the command, press Enter" |
| 8 | No cost information | Is this free? Will I be charged? | Add: "Claude Code uses Anthropic API credits. New accounts get $5 free credit" |

### Section: Creating Your App

| # | Location | Novice Confusion | Improvement |
|:-:|:---------|:-----------------|:------------|
| 9 | "Create a new folder" | How do I create a folder from terminal? | Add: "You can create the folder normally (right-click → New Folder), or type `mkdir my-mba-app`" |
| 10 | `cd path/to/my-mba-app` | What's my actual path? | Add concrete example: "Example: `cd ~/Desktop/my-mba-app` or `cd /Users/yourname/Documents/my-mba-app`" |
| 11 | "navigate to that folder" | What does navigate mean in terminal? | Add: "`cd` means 'change directory' — it's how you move between folders in terminal" |
| 12 | "Start Claude Code by typing: claude" | What should I see? How do I know it worked? | Add: "You should see Claude's welcome message and a prompt waiting for your input" |
| 13 | No mention of first-time setup | Claude Code asks for API key on first run | Add: "First time: Claude will ask for your Anthropic API key. Paste it when prompted" |
| 14 | "typically takes 1-3 minutes" | What do I do while waiting? Can I type? | Add: "Wait for Claude to finish. You'll see it creating files. Don't type until it asks for input" |
| 15 | Example prompt | Can I copy-paste this exactly? | Add: "You can copy-paste this example prompt to test, or write your own for your project" |

### Section: Running Locally

| # | Location | Novice Confusion | Improvement |
|:-:|:---------|:-----------------|:------------|
| 16 | "Ask Claude Code: How do I run this locally?" | Do I type this in quotes? | Add: "Type exactly: `How do I run this locally?` (no quotes needed)" |
| 17 | `npm install` and `npm run dev` | Claude runs these, or do I? | Clarify: "Claude will run these commands for you. Just confirm when it asks" |
| 18 | "localhost:5173" | What's localhost? Where do I paste this? | Add: "Open any web browser (Chrome, Safari) and type `localhost:5173` in the address bar" |
| 19 | No mention of keeping terminal open | If I close terminal, app stops | Add: "Keep the terminal window open while testing. Closing it stops your app" |
| 20 | What if port is busy? | "Port already in use" error | Add: "If you see 'port in use', Claude will suggest a different port like 5174" |

### Section: Git & GitHub

| # | Location | Novice Confusion | Improvement |
|:-:|:---------|:-----------------|:------------|
| 21 | "Help me initialize git" | What exactly do I type? | Add: Type this prompt exactly: `Help me initialize a git repository and push this project to GitHub` |
| 22 | "Creating a repository on GitHub.com" | Do I need to do this manually? | Clarify: "Claude will give you a link to create the repo on GitHub. Follow that link" |
| 23 | git commands listed | Do I need to memorize these? | Add: "You don't need to memorize these—Claude runs them for you" |
| 24 | "connecting it to your local project" | What does this mean technically? | Simplify: "This links your folder to GitHub so changes can be uploaded" |
| 25 | Public vs Private repo | Which should I choose? | Add: "Choose 'Public' so TAs can access it. You can delete it after the course" |

### Section: Making Changes & Pushing

| # | Location | Novice Confusion | Improvement |
|:-:|:---------|:-----------------|:------------|
| 26 | "describe the changes you want" | How specific should I be? | Add examples: "Be specific: 'Add a red delete button in the top-right corner of each card'" |
| 27 | "have a conversation with it" | How many back-and-forths is normal? | Add: "2-3 iterations is normal. If stuck after 5, try rephrasing your request" |
| 28 | `git push origin main` | What's origin? What's main? | Add: "origin = GitHub, main = your primary branch. Claude handles this for you" |
| 29 | "permanently alters your repository" | Can I undo this? | Add: "Yes, you can undo with `git revert` but ask Claude to help if needed" |
| 30 | No mention of .gitignore | node_modules shouldn't be pushed | Add: "Claude usually creates a .gitignore file. If not, ask: 'Create a .gitignore for a Node project'" |

---

## ✅ Top 10 Improvements to Implement

Based on severity (blocks completion) and frequency (affects most novices):

| Priority | # | Issue | Why Critical |
|:--------:|:-:|:------|:-------------|
| 🔴 1 | 5 | API key not mentioned | **Blocks 100% of users** on first run |
| 🔴 2 | 13 | First-time setup | Confusion when Claude asks for key |
| 🔴 3 | 1 | "What's a terminal?" | Blocks users who've never opened Terminal |
| 🟠 4 | 10 | `cd path/to/folder` | Abstract path confuses novices |
| 🟠 5 | 2 | Node.js version | LTS vs Current confusion |
| 🟠 6 | 18 | localhost explanation | Users don't know where to paste URL |
| 🟠 7 | 8 | Cost information | Fear of unexpected charges |
| 🟡 8 | 19 | Keep terminal open | App stops unexpectedly |
| 🟡 9 | 4 | Troubleshooting | "command not found" panic |
| 🟡 10 | 25 | Public vs Private | TAs can't access private repos |

---

## 📝 Improved Instructions Document

Creating: `PM_Prototyping_with_Claude_Code_v2.md`

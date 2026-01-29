# PM Prototyping with Claude Code & GitHub
## Assignment Instructions (v2.0 — Novice-Friendly Edition)

> **Improvements in v2**: Added prerequisites checklist, API key setup, terminal basics, troubleshooting, and clearer step-by-step guidance based on novice testing.

---

## 📋 Before You Start: Prerequisites Checklist

Complete these **before** starting the assignment:

| Step | Tool | Action | Verify |
|:----:|:-----|:-------|:-------|
| 1 | **Node.js** | Download LTS version from [nodejs.org](https://nodejs.org) | Open Terminal, type `node --version` → should show `v18.x.x` or higher |
| 2 | **Git** | Download from [git-scm.com](https://git-scm.com) (use default install options) | Type `git --version` → should show version number |
| 3 | **GitHub** | Create free account at [github.com](https://github.com) | Can log in to github.com |
| 4 | **Anthropic API Key** | Sign up at [console.anthropic.com](https://console.anthropic.com), get API key | Save your key somewhere safe |
| 5 | **Claude Code** | In Terminal: `npm install -g @anthropic-ai/claude-code` | Type `claude --version` → should show version |

### 💰 Cost Information
- New Anthropic accounts get **$5 free credit**
- Building one prototype typically costs **$0.50–$2.00**
- You can monitor usage at console.anthropic.com

### 🖥️ What is Terminal?
- **Mac**: Search "Terminal" in Spotlight (Cmd+Space), or find it in Applications → Utilities
- **Windows**: Search "Command Prompt" or "PowerShell" in Start menu
- Terminal is where you type commands and press Enter to run them

---

## 🚀 Step 1: Set Up Your Project Folder

### 1.1 Create a folder for your project

You can do this the normal way (right-click → New Folder) or in Terminal:

```bash
mkdir my-mba-app
```

### 1.2 Open Terminal and navigate to your folder

```bash
cd ~/Desktop/my-mba-app
```

> **What's `cd`?** It means "change directory" — you're telling Terminal which folder to work in.
>
> **Find your path**: Right-click your folder → "Get Info" (Mac) or "Properties" (Windows) to see the full path.

### 1.3 Start Claude Code

```bash
claude
```

**First time only**: Claude will ask for your Anthropic API key. Paste the key you saved from Step 4 in prerequisites.

You should see Claude's welcome message. Now you can type requests in plain English.

---

## 🏗️ Step 2: Create Your App

### 2.1 Give Claude your requirements

Type (or copy-paste) a detailed prompt. Example:

```
Create a web app for MBA students to find study partners. The app should have:
1. A home screen showing available study groups with filters for course and time
2. A group detail screen showing members, meeting times, and a join button
3. A create group screen with fields for course name, meeting time, location, and maximum members

Use a professional blue color palette (#1a365d as primary). Make it mobile-responsive.
```

> **Tip**: The more detail you provide, the better the result. Include colors, layouts, and specific features.

### 2.2 Wait for Claude to build

- This takes **1–3 minutes**
- You'll see Claude creating files and writing code
- **Don't type anything** until Claude asks for input or finishes

### 2.3 Run your app locally

When Claude finishes, type:

```
How do I run this app locally?
```

Claude will run commands like `npm install` and `npm run dev`. When it gives you a URL (usually `http://localhost:5173`):

1. Open your web browser (Chrome, Safari, Firefox)
2. Type `localhost:5173` in the address bar
3. Press Enter — your app appears!

> **Keep Terminal open!** Closing Terminal stops your app. Open a new Terminal tab if you need to run other commands.

---

## 📤 Step 3: Push to GitHub

### 3.1 Initialize Git and connect to GitHub

Type this prompt:

```
Help me initialize a git repository and push this project to GitHub.
I want to create a PUBLIC repository so my TAs can access it.
```

Claude will:
1. Run `git init` to start tracking your project
2. Give you a link to create a new repository on GitHub
3. Guide you through connecting your local folder to GitHub

### 3.2 Follow Claude's instructions

When Claude gives you a GitHub link:
1. Click the link (or copy-paste to browser)
2. Name your repository (e.g., `mba-study-partner-app`)
3. Select **Public** (so TAs can access)
4. Click "Create repository"
5. Come back to Terminal and tell Claude you're done

### 3.3 Verify on GitHub

Go to `github.com/YOUR-USERNAME/YOUR-REPO-NAME` — you should see all your files!

---

## ✏️ Step 4: Make Changes

### 4.1 Describe what you want to change

Just tell Claude in plain English:

```
Add a red delete button in the top-right corner of each study group card
```

```
Put the MIT Sloan logo in the header on the left side.
Use this URL: https://example.com/mit-logo.png
```

```
Add a confirmation dialog that asks "Are you sure?" when users click delete
```

### 4.2 Be specific

| ❌ Vague | ✅ Specific |
|:---------|:-----------|
| "Add a logo" | "Add the MIT logo to the top-left of the header" |
| "Make it look better" | "Change the background to light gray (#f5f5f5) and add more padding" |
| "Fix the button" | "Make the submit button blue (#1a365d) and increase its size" |

### 4.3 Iterate if needed

If Claude doesn't get it right the first time, clarify:

```
That's close, but move the logo to the left side of the text, not above it
```

> **Normal**: 2–3 iterations to get something right. If stuck after 5 tries, rephrase your request completely.

---

## 📤 Step 5: Push Your Changes

### 5.1 Commit and push

After making changes, type:

```
Commit my changes and push to GitHub with the message "Add delete button and confirmation dialog"
```

Claude will run the Git commands for you:
- `git add .` — stages your changes
- `git commit -m "your message"` — saves a snapshot
- `git push origin main` — uploads to GitHub

### 5.2 Verify on GitHub

Refresh your GitHub repository page. You should see your new commit message and updated files.

---

## 🎯 Final Deliverable

Share your **public GitHub repository URL** with your TAs:

```
https://github.com/YOUR-USERNAME/YOUR-REPO-NAME
```

Make sure:
- [ ] Repository is set to **Public**
- [ ] All your code is pushed (check GitHub shows your files)
- [ ] App runs locally with `npm run dev`

---

## 🔧 Troubleshooting

| Problem | Solution |
|:--------|:---------|
| `npm: command not found` | Install Node.js from nodejs.org, then restart Terminal |
| `git: command not found` | Install Git from git-scm.com, then restart Terminal |
| `claude: command not found` | Run `npm install -g @anthropic-ai/claude-code` again |
| "Port already in use" | Claude will suggest a different port (5174, etc.) |
| App stopped working | You probably closed Terminal. Run `npm run dev` again |
| API key error | Check your key at console.anthropic.com, paste it again when Claude asks |
| "Permission denied" | On Mac, try: `sudo npm install -g @anthropic-ai/claude-code` |
| Can't push to GitHub | Make sure you created the repo and followed Claude's connection steps |

---

## 💡 Tips for Success

1. **Be specific** — Detailed prompts get better results
2. **Iterate** — It's normal to refine requests 2–3 times
3. **Commit often** — Push to GitHub regularly so you don't lose work
4. **Test everything** — Click through all screens before submitting
5. **Ask for explanations** — Type "Explain how this app works" anytime
6. **Keep Terminal open** — Your app stops if you close it

---

## 🆘 Still Stuck?

Email your TAs with:
1. What you were trying to do
2. The exact error message (screenshot helps)
3. What you already tried

We're happy to help!

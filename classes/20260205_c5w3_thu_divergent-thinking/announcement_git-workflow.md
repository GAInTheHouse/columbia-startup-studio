# Team Submission Instructions — Due Friday, February 6

## What You're Submitting

Each team needs to submit the following to the class GitHub repo:

1. **Team README** — Team name and list of all member UNIs
2. **All ideas generated today** — FigJam exports, photos of sticky notes, text notes (LLMs can read photos of sticky notes, so don't worry about transcribing)
3. **Lean Canvases** — Screenshots or text of your AI-generated canvases

I'll use your submissions to generate another AI podcast with personalized feedback on your ideas and canvases.

### About Markdown (.md) Files

All text files should be submitted in **Markdown format** (`.md` extension). Markdown is a simple text format that's easy to read and write:

- `# Heading` for titles
- `## Subheading` for sections
- `- item` for bullet points
- `**bold**` for emphasis

You can write Markdown in any text editor — just save the file with a `.md` extension. GitHub will automatically render it nicely. It's also quickly becoming the native formatting system for LLMs. LLMs consume it very well and produce it easily if asked. For a quick reference, see [Markdown Guide](https://www.markdownguide.org/cheat-sheet/).

---

## Step-by-Step Git Instructions

### Step 1: Clone the repo (first time only)

Open your terminal and run:

```bash
git clone git@github.com:kenxle/columbia-startup-studio-public.git
cd columbia-startup-studio-public
```

> **Note:** GitHub requires SSH for pushing. If you haven't set up SSH keys, see [GitHub's SSH guide](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account).

If you've already cloned it before, pull the latest changes instead:

```bash
cd columbia-startup-studio-public
git pull origin main
```

### Step 2: Create a branch for your team

Do NOT work directly on `main`. Create a new branch:

```bash
git checkout -b team/your-team-name
```

Replace `your-team-name` with your actual team name (lowercase, use hyphens instead of spaces). For example:

```bash
git checkout -b team/pixel-pirates
```

### Step 3: Create your team folder

Inside the `teams/` directory, create a folder for your team, and a dated subfolder for today's submission:

```bash
mkdir -p teams/your-team-name/20260206
```

Your folder structure should look like:

```
teams/
  your-team-name/
    README.md              ← team name + member UNIs
    20260206/
      ideas.md             ← all ideas from today's exercises
      canvases.md          ← lean canvases (text or screenshots)
      photos/              ← sticky note photos, FigJam exports, etc.
```

### Step 4: Add your team README

Create a `README.md` inside your team folder (not the dated folder) with your team info:

```markdown
# Team Name

## Members
- Name (UNI)
- Name (UNI)
- Name (UNI)
- Name (UNI)
```

### Step 5: Add your files from today

Put all of today's work into the `20260206/` dated folder:

- **ideas.md** — All the ideas you generated (Exquisite Corpse scenarios, chatgpt output, dot voting results)
- **canvases.md** — Your Lean Canvases (paste text or embed screenshot links)
- **photos/** — Create this subfolder for any images (sticky note photos, FigJam screenshots, etc.)

```bash
# Create the photos subfolder if you have images
mkdir -p teams/your-team-name/20260206/photos

# Copy your photos in (adjust the path to where your photos are)
cp ~/Downloads/sticky-notes.jpg teams/your-team-name/20260206/photos/
```

### Step 6: Stage and commit your files

```bash
git add teams/your-team-name/
git commit -m "Add team submission: your-team-name"
```

### Step 7: Push your branch

```bash
git push -u origin team/your-team-name
```

### Step 8: Create a Pull Request

Go to the repo on GitHub: https://github.com/kenxle/columbia-startup-studio-public

You should see a banner saying your branch was recently pushed. Click **"Compare & pull request"**.

If you don't see the banner:

1. Click the **"Pull requests"** tab
2. Click **"New pull request"**
3. Set **base** to `main` and **compare** to `team/your-team-name`
4. Click **"Create pull request"**

For the PR title, use: `Add team: Your Team Name`

Then click **"Create pull request"**. I'll review and merge it.

---

## Alternate: GitHub Web Interface

If you're not comfortable with the command line, you can do everything through the GitHub website:

1. Go to https://github.com/kenxle/columbia-startup-studio-public
2. Click the branch dropdown (says "main") and type your branch name `team/your-team-name` — click "Create branch"
3. Navigate to the `teams/` folder
4. Click **"Add file" → "Create new file"**
5. Type `your-team-name/README.md` in the filename field (this creates the folder automatically)
6. Paste your team info and commit
7. Repeat for `your-team-name/20260206/ideas.md` and `your-team-name/20260206/canvases.md`
8. To upload photos: navigate to `your-team-name/20260206/`, click **"Add file" → "Upload files"**
9. Once all files are added, click **"Contribute" → "Open pull request"**

---

## Need Help?

- Google and LLMs are very good at git and should be able to solve your problems just by pasting them any errors you encounter. 
- If you're still having issues shoot me an email (krs2212). 

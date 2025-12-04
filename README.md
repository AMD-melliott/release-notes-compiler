# Release Notes Compiler

## Exercise Goal
Learn to use VS Code's split view and live Markdown preview while combining multiple files into a professional release notes document. This exercise simulates a real-world documentation workflow!

**What you'll learn:**
- Working with multiple files simultaneously in split view
- Using live Markdown preview to see formatting in real-time
- Writing well-formatted documentation with Markdown
- Creating professional release notes
- Efficient text editing and organization in VS Code

---

## Scenario

You're a Product Manager preparing for Version 1.0 launch! The development team has given you three separate text files with information about features, bug fixes, and credits. Your job is to combine them into a polished, well-formatted release notes document.

---

## Step-by-Step Instructions

### Step 1: Clone the Repository

Using your preferred method:

**Command Line:**
```bash
git clone https://github.com/AMD-melliott/release-notes-compiler.git
cd release-notes-compiler
```

**Or VS Code:**
1. `Ctrl+Shift+P` / `Cmd+Shift+P` → `Git: Clone`
2. Enter: `https://github.com/AMD-melliott/release-notes-compiler.git`
3. Open the cloned folder

---

### Step 2: Create a Branch

Let's create a branch for this work.

**Quick method:**
1. Click the branch name in the bottom-left (`main`)
2. Select **Create new branch**
3. Name it: `create-release-notes`

---

### Step 3: Explore the Source Files

You should see three text files in your workspace:
- `features.txt` - New features in version 1.0
- `bugs.txt` - Bug fixes in version 1.0
- `credits.txt` - Team members and acknowledgments

**Take a moment to open and read each file** to understand the content you'll be working with.

---

### Step 4: Set Up Split View

Now let's arrange VS Code to see multiple files at once.

1. **Open `features.txt`**
2. **Drag the tab to the right side** of the editor until you see a vertical split indicator

**[SCREENSHOT PLACEHOLDER: VS Code showing drag-to-split gesture with visual indicator]**

3. Release to create a split view
4. **Open `bugs.txt`** - it should open in the left pane
5. **Drag `bugs.txt` tab to the bottom** of the left pane to create a horizontal split

**[SCREENSHOT PLACEHOLDER: VS Code with 3-pane split view showing features, bugs, and credits files]**

6. **Open `credits.txt`** in the bottom-left pane

**Result:** You should now have all three source files visible at once!

**Alternative methods:**
- Right-click a tab → **Split Right** or **Split Down**
- `Ctrl+\` (Windows/Linux) or `Cmd+\` (Mac) to split current editor

**Learn more:** [VS Code Docs: Split editor](https://code.visualstudio.com/docs/getstarted/userinterface#_side-by-side-editing)

---

### Step 5: Create the Release Notes File

Now let's create your new Markdown file.

1. Click **File → New File** (or `Ctrl+N` / `Cmd+N`)
2. Save it immediately: **File → Save As** (or `Ctrl+S` / `Cmd+S`)
3. Name it: `v1.0_release_notes.md`
4. Make sure to include the `.md` extension!

**Why `.md`?** This tells VS Code it's a Markdown file, enabling syntax highlighting and preview features.

---

### Step 6: Open Markdown Preview

Here's where VS Code really shines for documentation work!

**Method 1: Command Palette**
1. With `v1.0_release_notes.md` open, press `Ctrl+Shift+P` / `Cmd+Shift+P`
2. Type `Markdown: Open Preview to the Side`
3. Select it from the list

**Method 2: Keyboard Shortcut**
- Press `Ctrl+K V` (Windows/Linux) or `Cmd+K V` (Mac)

**Method 3: Button**
- Look for the preview icon (📄🔍) in the top-right corner of the editor
- Click it to open preview

**[SCREENSHOT PLACEHOLDER: VS Code showing Markdown file on left with live preview on right]**

**What happened?** You now have a split view showing:
- **Left:** Your raw Markdown code
- **Right:** A live preview of how it will look when rendered

**The preview updates automatically as you type!**

**Learn more:** [VS Code Docs: Markdown preview](https://code.visualstudio.com/docs/languages/markdown#_markdown-preview)

---

### Step 7: Start Writing Your Release Notes

Let's begin with a basic structure. Type this into `v1.0_release_notes.md`:

```markdown
# Version 1.0 Release Notes

**Release Date:** [Add today's date]

We're excited to announce Version 1.0 of our product!

---

## What's New

[Features will go here]

---

## Bug Fixes

[Bug fixes will go here]

---

## Credits

[Credits will go here]

---

## Get Started

Download Version 1.0 today and explore these new features!
```

**Watch the preview pane update in real-time!** You should see:
- The `#` becomes a large heading
- `##` becomes a smaller section heading
- `---` becomes a horizontal line
- `**text**` becomes bold

**[SCREENSHOT PLACEHOLDER: Preview pane showing formatted release notes with headers and styling]**

---

### Step 8: Add Features Section

Now let's pull content from `features.txt` and format it properly.

1. Look at your split view with `features.txt`
2. Read through the features
3. In your release notes, replace `[Features will go here]` with formatted content:

```markdown
## What's New

### 🌙 Dark Mode Support
Users can now toggle between light and dark themes in the settings menu.

### 📄 Export to PDF
Documents can be exported directly to PDF format with a single click.

### 👥 Collaborative Editing
Real-time collaboration allows multiple users to edit documents simultaneously.

### 🔍 Advanced Search
Enhanced search functionality with regex support and filter options.

### 📋 Custom Templates
Users can create and save custom document templates for reuse.
```

**Markdown syntax you're using:**
- `###` - Third-level heading
- Emojis - Copy/paste or use your OS emoji picker
- Blank lines - Create spacing between sections

**Watch the preview!** See how each feature gets its own styled heading.

---

### Step 9: Add Bug Fixes Section

Now let's format the bug fixes as a clean list.

Replace `[Bug fixes will go here]` with:

```markdown
## Bug Fixes

This release includes the following bug fixes:

- Fixed crash when opening large files over 100MB
- Resolved memory leak in the auto-save feature
- Corrected rendering issues with special characters in titles
- Fixed synchronization problems in offline mode
- Resolved issue where undo history was lost after forced quit
- Corrected timezone display in document timestamps
- Fixed search highlighting not clearing properly
```

**Markdown syntax:**
- `- ` (dash + space) creates bullet points
- Each line becomes a list item

**Preview tip:** Notice how the list items are cleanly formatted with bullet points!

---

### Step 10: Add Credits Section

Finally, let's acknowledge the team with formatted lists and sections.

Replace `[Credits will go here]` with:

```markdown
## Credits

### Development Team
- **Sarah Chen** - Lead Developer
- **Michael Rodriguez** - Backend Engineer
- **Emily Watson** - Frontend Developer
- **James Park** - UI/UX Designer

### Quality Assurance
- **Lisa Thompson** - QA Lead
- **David Kumar** - Test Engineer

### Special Thanks
- Our beta testers for valuable feedback
- The open source community for tool support
- All users who reported issues and suggested improvements
```

**Markdown syntax:**
- `**Name**` makes names bold
- Nested lists with consistent indentation
- Blank lines between sections for readability

**[SCREENSHOT PLACEHOLDER: Completed release notes in preview showing all sections beautifully formatted]**

---

### Step 11: Polish Your Document

Now that you have all the content, add some finishing touches:

**At the top, add metadata:**
```markdown
---
**Version:** 1.0
**Release Date:** December 3, 2024
**Download:** [Get Version 1.0](https://example.com/download)
---
```

**At the bottom, add a call-to-action:**
```markdown
---

## Feedback

We'd love to hear from you! Report issues or suggest features on our [GitHub repository](https://github.com/example/repo).

Thank you for using our product! 🎉
```

---

### Step 12: Review Using Preview

Take a moment to review your work:

1. **Scroll through the preview pane**
2. Check that all sections are present:
   - Version info
   - Features with emojis
   - Bug fixes as a list
   - Credits with team names
   - Call-to-action
3. **Look for formatting issues:**
   - Missing blank lines between sections
   - Inconsistent heading levels
   - Typos or unclear wording

**Pro tip:** Click in the preview pane and scroll - it syncs with your editor position!

---

### Step 13: Save and Close Extra Files

Let's clean up your workspace.

1. **Save your release notes:** `Ctrl+S` / `Cmd+S`
2. **Close the source files** (`features.txt`, `bugs.txt`, `credits.txt`)
   - Right-click their tabs → Close
   - Or click the X on each tab
3. **Keep only:** `v1.0_release_notes.md` and its preview

**[SCREENSHOT PLACEHOLDER: Clean workspace with just the release notes and preview visible]**

---

### Step 14: Commit Your Work

Now let's save this to Git!

1. Open **Source Control** (`Ctrl+Shift+G` / `Cmd+Shift+G`)
2. You should see `v1.0_release_notes.md` as a new file (untracked)
3. **Stage the file** (click the + icon)
4. **Write a commit message:**
   ```
   Create v1.0 release notes

   - Compiled features from development team
   - Listed all bug fixes
   - Added credits and acknowledgments
   - Formatted using Markdown for readability
   ```
5. Click **✓ Commit**

---

### Step 15: Push and Create a Pull Request

1. **Push your branch:**
   - Click **⋯** → **Push**
   - Or click the sync icon in the status bar

2. **Create a PR on GitHub:**
   - Navigate to `https://github.com/AMD-melliott/release-notes-compiler`
   - Click **Compare & pull request**
   - Title: "Add v1.0 release notes"
   - Description:
     ```
     This PR adds professionally formatted release notes for v1.0 including:
     - 5 new features
     - 7 bug fixes
     - Team credits and acknowledgments
     ```
   - Click **Create pull request**

**Congratulations!** You've created a professional release notes document! 🎉

---

## Key Takeaways

- ✅ **Split view** enables efficient multi-file workflows
- ✅ **Live Markdown preview** shows formatting in real-time
- ✅ **Markdown syntax** is simple yet powerful for documentation
- ✅ **Good structure** makes release notes scannable and professional
- ✅ **VS Code** is excellent for documentation work, not just code

---

## Markdown Quick Reference

Here's what you learned:

| Syntax | Result |
|--------|--------|
| `# Heading 1` | Large heading |
| `## Heading 2` | Section heading |
| `### Heading 3` | Subsection heading |
| `**bold text**` | **bold text** |
| `*italic text*` | *italic text* |
| `- list item` | • list item |
| `1. numbered` | 1. numbered |
| `---` | Horizontal line |
| `[link](url)` | Clickable link |

**Learn more:** [Markdown Guide - Basic Syntax](https://www.markdownguide.org/basic-syntax/)

---

## Bonus Challenges

### Challenge 1: Add a Table of Contents
Use Markdown to create a clickable table of contents at the top:

```markdown
## Table of Contents
- [What's New](#whats-new)
- [Bug Fixes](#bug-fixes)
- [Credits](#credits)
```

The `#anchor-name` links to headings in your document!

### Challenge 2: Add a Comparison Table
Create a table comparing features across versions:

```markdown
## Feature Comparison

| Feature | Version 0.9 | Version 1.0 |
|---------|-------------|-------------|
| Dark Mode | ❌ | ✅ |
| PDF Export | ❌ | ✅ |
| Collaboration | ❌ | ✅ |
```

### Challenge 3: Add Code Blocks
If your product has API changes, document them:

```markdown
## API Changes

Initialize the new feature:
\`\`\`javascript
const app = new App({
  darkMode: true
});
\`\`\`
```

**Learn more:** [VS Code Markdown Extensions](https://marketplace.visualstudio.com/search?target=VSCode&category=Formatting&term=markdown)

---

## Troubleshooting

### "The preview isn't updating"
- Make sure you saved the file with `.md` extension
- Try closing and reopening the preview
- Check that you're editing the file, not the preview pane

### "I can't see the preview icon"
- Make sure the file has `.md` extension
- Try using `Ctrl+Shift+P` → `Markdown: Open Preview to the Side`

### "My split view is messy"
- Click **View → Editor Layout → Single** to reset
- Then rebuild your split view from scratch
- Or drag tabs to rearrange them

### "Markdown syntax isn't rendering"
- Make sure there are spaces after `#`, `-`, etc.
- Check for blank lines between sections
- Review the Markdown Quick Reference above

---

## Real-World Application

**This workflow is used daily for:**
- Product release notes (like you just created!)
- API documentation
- README files for GitHub projects
- Technical specifications
- User guides and tutorials
- Blog posts and articles

**Professional tip:** Many companies use this exact workflow with tools like:
- GitHub Pages (renders Markdown as websites)
- ReadTheDocs (documentation hosting)
- Jekyll/Hugo (static site generators)

---

## Additional Resources

- [Markdown Guide](https://www.markdownguide.org/)
- [VS Code Markdown Documentation](https://code.visualstudio.com/docs/languages/markdown)
- [GitHub Flavored Markdown Spec](https://github.github.com/gfm/)
- [Awesome Markdown](https://github.com/mundimark/awesome-markdown) - Tools and resources
- [Markdownlint Extension](https://marketplace.visualstudio.com/items?itemName=DavidAnson.vscode-markdownlint) - Linting for Markdown

---

## Example Release Notes for Inspiration

Want to see how real companies write release notes?

- [VS Code Release Notes](https://code.visualstudio.com/updates)
- [GitHub Release Notes](https://github.blog/changelog/)
- [Slack Release Notes](https://slack.com/release-notes)
- [Notion What's New](https://www.notion.so/releases)

---

**Next Exercise:** [Global Find & Replace](https://github.com/AMD-melliott/global-find-replace) - Master project-wide search and replace!

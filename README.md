# Website Project – Collaboration Guide

## 1. Project Structure

```text
website/
├── login.html
├── index.html
├── about.html
├── contact.html
├── style.css
├── script.js
├── assets/
│   ├── images/
│   ├── videos/
│   └── icons/
├── README.md
└── .gitignore
```

**File responsibilities:**
- `login.html` – Login interface.
- `index.html` – Main website and primary content.
- `about.html` – About the website and developers.
- `contact.html` – Contact information and form.
- `style.css` – All website styling.
- `script.js` – All JavaScript functionality.
- `assets/` – Images, videos, icons, and other media.

## 2. Design Guidelines

Follow these guidelines to maintain a consistent website across all pages.

### Typography
- **EB Garamond:** General website typography, headings, and primary text. https://fonts.google.com/specimen/EB+Garamond
- **Open Sans:** Text inside UI elements, including buttons, inputs, navigation, and forms. https://fonts.google.com/specimen/Open+Sans
- Maintain consistent font sizes and font weights.

### Border Radius
- **25px:** Large containers, sections, cards, and major divisions.
- **20px:** Smaller elements, including inputs, buttons, and other UI components.
- Keep border radius consistent throughout the website.

### General Design Rules
- Maintain consistent spacing, margins, and padding.
- Use the same navigation design across all pages.
- Follow the agreed color palette.
- Avoid unnecessary colors, fonts, and decorative elements.
- Keep layouts clean, readable, and responsive.
- Reuse existing CSS classes instead of creating duplicate styles.

## 3. Coding Conventions

- Use lowercase filenames.
- Use descriptive class and ID names.
- Use consistent indentation and formatting.
- Avoid inline CSS and JavaScript.
- Keep shared styles in `style.css`.
- Keep functionality in `script.js`.
- Add comments when implementing complicated sections.
- Check existing code before modifying shared elements.

Example:

```html
<div class="content-card">
    <h2 class="card-title">Welcome</h2>
    <p class="ui-text">Website description.</p>
</div>
```

## 4. Media Guidelines

Store all media inside `assets/`.

```html
<img src="assets/images/logo.png" alt="Logo">

<video controls>
    <source src="assets/videos/intro.mp4" type="video/mp4">
</video>
```

- Use descriptive filenames.
- Prefer optimized images and videos.
- Avoid unnecessarily large media files.
- Use relative paths instead of computer-specific file paths.

## 5. Collaboration Workflow

**VS Code + Live Share + GitHub**

1. Host opens the project folder in VS Code.
2. Host starts a Live Share session.
3. Partner joins through the invitation link.
4. Both can edit the shared workspace.
5. Use Live Server to preview changes.
6. Save changes using Auto Save or `Ctrl + S`.
7. Host reviews changes and commits them to GitHub.
8. Push the latest version to the repository.

**Important:** Live Share edits the host's workspace. It does not automatically create a permanent local copy on the partner's computer. GitHub is our backup and version history.

## 6. Essential Git Commands

Run these in the VS Code terminal.

| Command | Purpose |
|---|---|
| `git status` | Check modified files |
| `git add .` | Stage all changes |
| `git commit -m "message"` | Save a version |
| `git push` | Upload commits to GitHub |
| `git pull` | Download latest changes |
| `git log --oneline` | View commit history |

### Initial Setup (Host Only)

```bash
git init
git add .
git commit -m "Initial project setup"
git branch -M main
git remote add origin REPOSITORY_URL
git push -u origin main
```

### Regular Workflow

```bash
git status
git add .
git commit -m "Updated homepage layout"
git push
```

Before starting a new independent work session:

```bash
git pull
```

**Avoid editing and committing the same files independently from different computers without coordinating first.**

## 7. Final Reminders

- Communicate before changing shared designs or components.
- Don't overwrite your partner's unfinished work.
- Test navigation and links after modifications.
- Keep the website functional before adding optional features.
- Commit completed work regularly.
- Always maintain consistency with the design guidelines.

**Goal: One unified website, not four independently designed webpages.**

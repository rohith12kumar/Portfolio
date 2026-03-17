# Rohith Kumar Mamindla — Portfolio Edit Guide

## File Structure
```
index.html        ← The entire portfolio (open this in browser)
EDIT_GUIDE.md     ← This guide
rohith.jpg        ← Your hero/beach photo (backup)
pass_photo.jpg    ← Your passport/about photo (backup)
```

## How to Edit

### Open the file
- Open `index.html` in VS Code or any text editor
- Use Ctrl+F (Find) to locate the section you want to change

---

## Quick Edits — Search for these strings

### Personal Info
| What to change | Search for |
|---|---|
| Your name | `Rohith Kumar` |
| Your email | `rohithkumarmamindla12@gmail.com` |
| Phone number | `+91 9392676502` |
| GitHub link | `rohith12kumar` |
| LinkedIn link | `rohith12kumar` |

### Hero Section
- **Tagline/role**: Search `Backend Developer` → change text after `hero-role`
- **Description**: Search `B.Tech CSE graduate` → edit the paragraph
- **Stats (2+, 4, 7.2)**: Search `hero-stats` → change numbers in `stat-num` divs

### About Section
- **Bio paragraph**: Search `Computer Science graduate from Parul`
- **Education**: Search `B.Tech — Computer Science Engineering`
- **CGPA**: Search `CGPA: 7.2`
- **Certifications**: Search `Java Full Stack` — 4 cert items below it

### Skills Section
- Each skill card has a `<h4>` title and `<div class="skill-tags">` with spans
- Search `Backend Development` to find skill cards
- Tag colors:
  - `.tag` = green (built projects with)
  - `.tag training` = yellow (completed training)
  - `.tag learning` = blue (currently learning)

### Projects Section
- Search `Green Basket` to find first project
- Search `Campus Connect` to find second project
- To **add a project**: Copy a `<div class="project-card">` block and paste after

### Journey/Timeline
- Search `Started B.Tech` to find the timeline
- Each timeline item is a `<div class="tl-item">` block

### Contact Section
- Search `Let's Connect` to find contact section

---

## Adding a New Project

Copy this template and paste inside `<div class="projects-grid">`:

```html
<div class="project-card">
  <div class="project-img">🚀</div>
  <div class="project-body">
    <h3>Your Project Name</h3>
    <p>Brief description of what it does and what you built.</p>
    <div class="project-tech">
      <span class="tag">Python</span>
      <span class="tag">MySQL</span>
    </div>
    <div class="project-links">
      <a href="YOUR_GITHUB_LINK" target="_blank">GitHub</a>
      <a href="YOUR_LIVE_LINK" target="_blank">Live Demo</a>
    </div>
  </div>
</div>
```

---

## Changing Colors

At the top of the file, inside `<style>`, find `:root { ... }`:

```css
:root {
  --teal: #00d4aa;    ← Main accent color (change this)
  --cyan: #00cfe8;    ← Secondary accent
  --bg:   #0a0a0f;    ← Page background
  --text: #e8e8f0;    ← Main text color
}
```

---

## Deploying

**Netlify (Free — 60 seconds):**
1. Go to https://netlify.com/drop
2. Drag `index.html` into the browser
3. Get a live URL instantly

**GitHub Pages:**
1. Create a new GitHub repo
2. Upload `index.html` (rename if needed)
3. Settings → Pages → Deploy from main branch

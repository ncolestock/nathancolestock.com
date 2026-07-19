# nathancolestock.com

Personal website — single timeline page with typewriter/legal pad aesthetic.

Built with vanilla HTML/CSS/JS. No framework, no build step. Deployable to any static host.

## Content

Entries are hardcoded in `index.html` inside the `<script>` tag as an array of objects with:
- `date` — display date
- `type` — Devotional, Sermon, Essay, Letter, Article, Reflection
- `title` — entry title
- `toc` — array of section headings for the table of contents
- `body` — HTML content (template literal)

## Design

- Typewriter monospace font (Courier New / IBM Plex Mono)
- Legal pad lined-paper background
- Collapsible expand/collapse entries
- Brown accent (#8b4513)
- Responsive down to mobile

## Deployment

This repo is ready for GitHub Pages or any static host. To deploy:

1. Add the SSH key to GitHub: `cat ~/.ssh/id_ed25519.pub` → GitHub Settings → SSH Keys
2. Create a repo called `nathancolestock.com` on GitHub
3. `git remote add origin git@github.com:nathancolestock/nathancolestock.com.git && git push -u origin main`
4. Enable GitHub Pages in repo Settings → Pages → Source: deploy from main branch, root directory
5. Point nathancolestock.com DNS to GitHub Pages IPs or configure a CNAME

## Status

- Content and design rework tracked in kanban task t_4db91c5c
- Deployment infra tracked in kanban task t_0000003b

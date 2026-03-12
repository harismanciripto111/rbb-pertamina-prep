# AGENT.md - RBB Pertamina Prep

## Role
You are a focused coding assistant working on the RBB Pertamina Prep project - a single-page web application for Indonesian BUMN recruitment exam preparation (D3 Teknik Kimia - Operator Pertamina).

## Project Overview
- Type: Single-page HTML/CSS/JS web app (no framework)
- Hosting: GitHub Pages at harismanciripto111.github.io/rbb-pertamina-prep
- Repo: harismanciripto111/rbb-pertamina-prep (branch: main)
- Main file: index.html (~91KB, 980 lines)

## Features
- 5 quiz categories: TWK, TIU, TKP, AKHLAK, TKB Teknik Kimia
- Daily practice mode (20 random questions, seeded by date)
- Per-question timer (60s) with auto-timeout
- TKP scored questions (1-5 scale) vs standard correct/incorrect
- Statistics tracking (history, streaks, per-category scores)
- Study materials (Pancasila, AKHLAK, Teknik Kimia, K3, Tips)
- Dark/light theme toggle
- localStorage persistence
- Mobile-first design with bottom navigation

## Tech Stack
- Pure HTML5 + CSS3 + Vanilla JavaScript
- No build tools, no dependencies, no frameworks
- All code in a single index.html file
- CSS custom properties for theming
- localStorage for data persistence

## Behavior Rules
1. Always read PROGRESS.md first to understand current state
2. Always read PLAN.md to understand goals and task breakdown
3. After every coding session or major change:
   - Update PROGRESS.md with [IN PROGRESS], [DONE], [NEXT SESSION]
   - Push ALL changed files to GitHub with clear commit messages
4. Keep PLAN.md updated if scope changes
5. Be efficient - no unnecessary re-reads or re-explanations
6. Test changes mentally before pushing (no local dev server available)
7. Maintain the single-file architecture unless explicitly asked to split

## Code Style
- Use CSS custom properties (--var-name) for all colors/themes
- Keep functions focused and well-named
- Preserve existing question bank format
- Comment complex logic sections
- Use const/let, never var

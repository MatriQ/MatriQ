# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is a GitHub profile repository for Matri Qi (MatriQ), containing a personal profile README and automated GitHub Actions workflows.

## Repository Structure

- `README.md` - Personal profile showcasing professional experience, tech stack, education, and achievements
- `.github/workflows/snake-ani.yaml` - GitHub Actions workflow that generates contribution graph snake animations

## GitHub Actions

### Snake Animation Workflow
The repository uses `Platane/snk@v3` to generate animated snake visualizations of GitHub contributions.

**Trigger**:
- Scheduled: Runs every 12 hours (`0 */12 * * *`)
- Manual: Via `workflow_dispatch`

**Output**: Generates snake animation files to the `output` branch:
- `github-snake.svg` (default theme)
- `github-snake-dark.svg` (dark palette)
- `ocean.gif` (custom color scheme)

**Manual trigger**:
```bash
# Trigger via GitHub CLI
gh workflow run snake-ani.yaml
```

## README.md

The README contains:
- Professional profile with contact information (Email, LinkedIn)
- Language proficiencies (Python, TypeScript, Golang, JavaScript, C++, SQL, Lua)
- Tech stack badges and icons (React, Node.js, FastAPI, Flask, K8s, Docker, PostgreSQL, Redis, Next.js, NestJS, Prisma, Unity, Three.js)
- Work experience at bitHuman Inc and AiFi Inc
- Education history (MBA from Southwest University, Network Engineering degree)
- Honors and awards (Dify contributor, Microsoft competition wins)
- Embedded snake animation visualization

When updating the README, maintain the existing visual formatting style with:
- Badge images for skills and contact information
- DevIcon CDN links for tech stack icons
- Capsule Render for the header banner
- Snake animation references using the `<picture>` element for theme support

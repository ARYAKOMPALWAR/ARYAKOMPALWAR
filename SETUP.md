# GitHub Profile Setup Guide

## Step 1: Create the profile repo

1. Go to https://github.com/new
2. Name the repository exactly: `ARYAKOMPALWAR` (your GitHub username)
3. Set it to **Public**
4. Do **not** initialize with README, .gitignore, or license
5. Click **Create repository**

## Step 2: Upload files

Upload the following files to the root of the new repo:

| File | Destination in repo |
|------|---------------------|
| `README.md` | Root `/README.md` |
| `assets/banner.svg` | `/assets/banner.svg` |
| `.github/workflows/contributions-snake.yml` | `.github/workflows/contributions-snake.yml` |
| `.gitignore` | `.gitignore` |

GitHub will automatically render `README.md` as your profile page.

## Step 3: What to customize

### README.md replacements
- `ARYAKOMPALWAR` — your GitHub username (already set)
- `Building X`, `Learning Y`, `Shipping Z` — update the status chip text
- Project repo links — replace `https://github.com/ARYAKOMPALWAR` with each project's actual repo URL:
  - ContribuX: `https://github.com/ARYAKOMPALWAR/ContribuX`
  - Sudharna: `https://github.com/ARYAKOMPALWAR/Sudharna` (or your repo name)
  - Gen AI app: `https://github.com/ARYAKOMPALWAR/gen-ai-app` (or your repo name)

### Banner
- Replace `assets/banner.svg` with your own banner image if desired (keep it 1200×400 px)
- The current SVG uses twinkling stars and a green accent — swap it for a screenshot or custom artwork if you have one

### Snake workflow
- The workflow uses `ARYAKOMPALWAR` as the GitHub username. If your username differs, update `github_user_name` in `.github/workflows/contributions-snake.yml`
- After the first push, the workflow runs automatically and commits `dist/*.svg` back to the repo
- The snake image in README.md points to `raw.githubusercontent.com/ARYAKOMPALWAR/ARYAKOMPALWAR/output/snake.svg` — adjust the path if your repo name differs

## Step 4: Enable GitHub Pages (optional)

If you want a live portfolio site at `aryakompalwar.github.io`:
1. Repo → **Settings** → **Pages**
2. Source: **Deploy from a branch**
3. Branch: `main` / root
4. Save. Your site will be live at `https://aryakompalwar.github.io/ARYAKOMPALWAR/`

## Notes

- GitHub strips `<style>` and `<script>` from READMEs, so animations are limited to image assets (banner SVG, snake GIF/SVG)
- The badge images are from `img.shields.io` — if they don't load, they degrade gracefully to text
- Keep `assets/` and `.github/` folders in the repo for the workflow to function

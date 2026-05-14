# Repository Guidelines

## Project Structure & Module Organization
This repository is a Jekyll-based portfolio site for GitHub Pages. Core content lives in `index.md`, which serves as the main landing page. Shared site settings are in `_config.yml`, navigation is in `_data/navigation.yml`, and the only standalone page currently tracked is `_pages/404.md`. Keep styling changes centralized in `assets/css/main.scss`, and store static media under `assets/images/`. Record notable edits in `작업기록.md`.

## Build, Test, and Development Commands
Install dependencies with `bundle install`. Run the site locally with `bundle exec jekyll serve` and review it at `http://127.0.0.1:4000`. Use `bundle exec jekyll build` before opening a PR to catch Liquid, Markdown, or config errors that would break GitHub Pages. Deployment is handled automatically by `.github/workflows/jekyll.yml` on pushes to `main`.

## Coding Style & Naming Conventions
Write concise Markdown focused on outcomes, numbers, and scope rather than vague task descriptions. Prefer short sections and clear headings in `index.md`. Use 2-space indentation in YAML files such as `_config.yml` and `_data/navigation.yml`. Keep CSS minimal, readable, and scoped; avoid broad overrides and avoid `!important`. Follow existing Jekyll naming patterns such as underscore-prefixed directories (`_pages`, `_data`) and lowercase asset paths like `assets/images/bio-photo.jpg`.

## Testing Guidelines
There is no separate automated test suite in this repository. The required validation step is a clean `bundle exec jekyll build`. When editing layout, copy, or navigation, also verify the local rendered page and confirm links, section anchors, and Korean text render correctly.

## Commit & Pull Request Guidelines
Recent history uses short Korean summaries such as `CODEX 리팩토링 5`; continue with brief, imperative commit messages that describe the user-facing change, for example `포트폴리오 소개 문구 정리`. Keep unrelated content, style, and config edits in separate commits when practical. PRs should include a short summary, affected files, local build status, and screenshots when visual output changes.

## Repository-Specific Workflow Notes
Before making larger edits, review `README.md`, `작업기록.md`, `_config.yml`, `index.md`, `_data/navigation.yml`, and `assets/css/main.scss`. Any meaningful content, structure, or styling change should be appended to `작업기록.md` with the date, changed files, reason, and user impact.
If work needs to reference or coordinate with Obsidian notes, use the vault path `C:\Users\AM11D\Documents\NockChaWang`.

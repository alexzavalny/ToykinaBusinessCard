# Repository Guidelines

## Project Structure & Module Organization
Main Jekyll config lives in `_config.yml`. Layouts sit in `_layouts/*.html` and reusable Liquid snippets in `_includes/`. Markdown content resides in `_posts`, `_services`, `_products`, and supplemental data files under `_data`. Public-facing pages (such as `about-me/`, `services/`, `blog/`) contain page-specific markdown plus optional assets. Styles and scripts originate in `assets/` with SCSS partials stored in `_sass` and compiled CSS emitted to `css/`. Images stay in `img/` (hero shots in `img/hero/`). The generated `_site/` directory is build output only—never edit or commit it directly.

## Build, Test, and Development Commands
- `bundle install` – install Ruby gems from `Gemfile`.
- `bundle exec jekyll serve --livereload` – build and host the site at `http://localhost:4000` for iterative edits.
- `bundle exec jekyll build` – produce a production-ready `_site` folder and fail fast on Liquid or front-matter issues.
- `bundle exec jekyll doctor` – lint the configuration for deprecated or conflicting settings.

## Coding Style & Naming Conventions
Indent HTML, Liquid, and YAML with two spaces. Use kebab-case filenames (e.g., `_posts/2024-05-12-care-plan.md`, `_services/sensory-coaching.md`) and keep the slug aligned with the `permalink`. Keep front matter minimal but complete (`layout`, `title`, `date`, `categories`, `image`). SCSS partials belong in `_sass` and are imported via `assets/css/main.scss`; avoid inline styles in layouts. Assets referenced in markdown should use absolute paths (`/img/hero/example.jpg`) to respect Jekyll’s baseurl handling.

## Testing Guidelines
No dedicated automated test suite ships with this repo, so treat `bundle exec jekyll build` as the smoke test before every push. Manually verify critical pages in the served site (`http://localhost:4000/about-me/`, `/services/`, `/blog/`) and confirm hero images load and navigation links resolve. When adding posts, ensure the filename timestamp matches the `date` field so chronological ordering remains stable.

## Commit & Pull Request Guidelines
Commits in this repo favor concise imperative subjects (“add blog post”, “tweak hero spacing”); follow that pattern and keep scopes small. Pull requests should summarize the change, call out new or renamed content files, include screenshots or GIFs for visual changes, and link any relevant issue or request. Mention any deployment considerations (new assets, config tweaks) so reviewers can re-run `bundle exec jekyll build` as needed.

## Content & Deployment Tips
Adjust `_config.yml` when updating navigation or social links, and sync `_data` files with any new repeating sections (services, products). Upload media to `img/` or nested folders and compress before commit. Deployments trigger automatically on pushes to `main`, so only merge once the local build and spot checks pass.

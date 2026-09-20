# GitHub Profile Setup — digital-mahesh

This package is designed for the special GitHub profile repository:

`digital-mahesh`

## Files

- `README.md` — the complete interactive profile page
- `.github/workflows/snake.yml` — automatically generates the contribution snake
- `output/` — created automatically by GitHub Actions after the workflow runs

## Setup

### 1. Create the profile repository

On GitHub, create a **public repository** named exactly:

`digital-mahesh`

GitHub will recognize it as your profile repository because it matches your username.

### 2. Upload these files

Upload:

```text
README.md
.github/
└── workflows/
    └── snake.yml
```

You do not need to create the `output` folder manually.

### 3. Enable Actions

Go to:

`Repository → Settings → Actions → General`

Make sure GitHub Actions are allowed to run.

The workflow needs permission to commit the generated SVG into the repository. The workflow file already requests:

```yaml
permissions:
  contents: write
```

### 4. Run it once manually

Open:

`Actions → Generate contribution snake → Run workflow`

After it finishes, an `output/` directory containing the snake SVG should appear.

### 5. Replace the LinkedIn placeholder

In `README.md`, find:

`YOUR_LINKEDIN_USERNAME`

and replace it with your real LinkedIn username.

### 6. Replace the email placeholder

Find:

`YOUR_EMAIL@example.com`

and replace it with the email address you want displayed publicly.

## Important GitHub limitation

GitHub profile READMEs cannot run arbitrary JavaScript. The "interactive" feel here is therefore created with:

- clickable navigation
- collapsible `<details>` sections
- live/generated statistics
- animated typing text
- contribution animation
- activity graph
- live badges
- project demo/source links
- responsive image-based components

This is safer and more compatible than trying to inject JavaScript into a GitHub README.

## Recommended pinned repositories

Pin the repositories that best represent your work. A strong starting set is:

1. `cutora-ai-background-remover`
2. `roadsewa-road-maintenance-portal`

As you build more AI/ML projects, replace older pins with stronger projects.

## Profile design principle

The README intentionally avoids:

- fake job titles
- exaggerated AI expertise
- claiming unfinished projects are completed
- huge walls of badges
- student-status-heavy wording

The goal is a developer profile that can evolve naturally as your AI/ML portfolio grows.

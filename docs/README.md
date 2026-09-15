# Emoji Match Game
> A browser-based memory game where players match pairs of emojis.

### authorship + version

`@Jake-Thrasher` | `2026-09-15` | `GOLF`

### deployments, codebase, & repo features 

| resource | link |
|---|---|
| PROD codebase | [`main`](https://github.com/Jake-Thrasher/matching-game/tree/main) |
| PROD server | [GCP](http://34.123.165.98) |
| DEV codebase | [`dev`](https://github.com/Jake-Thrasher/matching-game/tree/dev) |
| DEV server | [Render](https://matching-game-gula.onrender.com/) |
| docs | [`docs/`](https://github.com/Jake-Thrasher/matching-game/tree/main/docs) |
| published docs | [GitHub Pages](https://jake-thrasher.github.io/matching-game/) |
| CI/CD workflow | [`deploy.yml`](https://github.com/Jake-Thrasher/matching-game/blob/main/.github/workflows/deploy.yml) |
| successful PROD deployment | [GitHub Action](https://github.com/Jake-Thrasher/matching-game/actions) |
| resolved GOLF issue | [issue #1](https://github.com/Jake-Thrasher/matching-game/issues/1) |

### user story

- **As a** full-stack developer,
- **I want** to use a CI/CD infrastructure to manage and deploy my Emoji Match Game,
- **so that** I can develop locally, manage my code in GitHub, and automatically deploy updates to DEV and PROD environments.

### narrative

The Emoji Match Game is a web application that allows users to flip cards and find matching emoji pairs. I developed the application locally and stored the project in GitHub so that I could manage the code using separate `dev` and `main` branches. The `dev` branch is deployed to Render for testing, while the `main` branch uses GitHub Actions to automatically deploy updates to a Google Cloud Platform virtual machine for production.

### architecture

``` text
LOCAL
  │
  ▼
GitHub
  │
  ├── dev  ──► Render ─────────► DEV
  │
  └── main ──► GitHub Actions ─► GCP ──► PROD
stack

HTML/CSS/JS

	

Node.js

	

Express

	

Git/GitHub

	

Render

	
project structure
matching-game/
├── .github/
│   └── workflows/
│       └── deploy.yml
├── docs/
│   └── README.md
├── public/
│   ├── img/
│   │   └── Webframe_app.pdf
│   ├── scripts/
│   │   └── gameScripts.js
│   ├── styles/
│   │   └── gameStyles.css
│   └── index.html
├── server/
│   └── server.js
├── .gitignore
├── package-lock.json
├── package.json
└── README.md
GCP

external IP: 34.123.165.98 Linux user: jakethrasher01 instructor SSH public key installed: yes

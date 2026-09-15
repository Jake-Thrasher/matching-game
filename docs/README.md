# Emoji Match Game

## Tagline

A simple memory matching game where players match pairs of emojis and earn points.

## Author and Version

- **Author:** Jake Thrasher
- **Version:** 1.0
- **Course:** GOLF Deployment Assignment
- **Repository:** https://github.com/Jake-Thrasher/matching-game

## Deployment Links

- **Development:** https://matching-game-gula.onrender.com/
- **Production:** http://34.123.165.98
- **GitHub Repository:** https://github.com/Jake-Thrasher/matching-game
- **Successful GitHub Actions Run:** Add the successful Actions URL here

## User Story

As a player, I want to enter my name and match emoji cards so that I can earn points and try to get a high score.

## Application Narrative

The Emoji Match Game is a browser-based memory game. The player enters a name and starts the game. The application displays hidden emoji cards in a grid. The player selects two cards at a time to find matching pairs. Matching cards stay visible and increase the score. Incorrect matches are hidden again and decrease the score. The reset button allows the player to start over.

## Architecture

The application uses a client-server architecture. The frontend files are stored in `public/`. The Express server is stored in `server/`. Node.js and Express serve the frontend files. Nginx forwards public web traffic to Express, and PM2 keeps the application running on the GCP virtual machine.

## Technology Stack

- HTML
- CSS
- JavaScript
- jQuery
- Bootstrap 5
- Node.js
- Express
- Nginx
- PM2
- GitHub
- GitHub Actions
- Google Cloud Platform
- Render

## Project Tree

```text
matching-game/
├── .github/
│   └── workflows/
│       └── deploy.yml
├── docs/
│   └── README.md
├── public/
│   ├── img/
│   ├── scripts/
│   ├── styles/
│   └── index.html
├── server/
│   └── server.js
├── .gitignore
├── package-lock.json
├── package.json
└── README.md

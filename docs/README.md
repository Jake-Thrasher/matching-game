# Emoji Match Game

## Tagline

A simple memory matching game where players match pairs of emojis and earn points.

## Author and Version

- **Author:** Jake Thrasher
- **Version:** 1.0
- **Course:** GOLF Deployment Assignment
- **Repository:** https://github.com/Jake-Thrasher/matching-game

## Deployment Links

- **Development:** Render deployment link will be added
- **Production:** http://34.123.165.98
- **GitHub Repository:** https://github.com/Jake-Thrasher/matching-game

## User Story

As a player, I want to enter my name and match emoji cards so that I can earn points and try to get a high score.

## Application Narrative

The Emoji Match Game is a browser-based memory game. The player enters a name and starts the game. The application displays hidden emoji cards in a grid. The player selects two cards at a time to find matching pairs. Matching cards stay visible and increase the score. Incorrect matches are hidden again and decrease the score. The reset button allows the player to start over.

## Architecture

The application uses a simple client-server architecture.

- The frontend is made with HTML, CSS, JavaScript, jQuery, and Bootstrap.
- The frontend files are stored in the `public/` folder.
- The Express server is stored in the `server/` folder.
- Node.js and Express serve the frontend files.
- Nginx receives public web requests and forwards them to the Express server.
- PM2 keeps the Node.js application running on the GCP virtual machine.
- GitHub is used for source control and deployment workflows.

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
├── docs/
│   └── README.md
├── img/
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

# Boardgame Narrator

Boardgame Narrator is a lightweight static web app for running two tabletop-game helper screens:

- Avalon game assistant
- Werewords game assistant

Everything runs as plain HTML, CSS, and JavaScript in the browser. There is no build step or backend required.

## Project structure

- `index.html` — entry page that lets you choose a game helper
- `avalon.html` — Avalon narrator and mission tracker
- `werewords.html` — Werewords narrator with hidden word flow and timer

## Features

### Avalon helper

- Add and remove players
- Select which hidden roles are in play
- Narrate the night phase with browser speech synthesis
- Track mission participation round by round
- Keep a simple mission history log
- Toggle between light and dark theme

### Werewords helper

- Select special roles (Seer, Minion, Fortune Teller)
- Enter the secret magic word privately as the village leader
- Reveal the word during the night flow with optional spoken narration
- Use a spoken-night sequence to guide the game
- Start a countdown timer for 3, 4, or 5 minutes
- Reset the current match and restart setup easily

## How to use

1. Open `index.html` in a browser.
2. Choose either the Avalon or Werewords tool.
3. Follow the on-screen steps for that game.
4. For best results, use a browser with speech synthesis support (Chrome/Edge recommended).

## Local preview

You can also run a quick local server from the project folder:

```bash
python -m http.server 8000
```

Then open:

```text
http://localhost:8000/
```

## Notes

- The app stores theme preferences in `localStorage`.
- This project is intentionally simple and portable; it is designed for local, in-person tabletop sessions.
- No external dependencies or package installation are needed.

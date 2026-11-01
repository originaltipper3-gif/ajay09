# Toss King Ajay — Telegram Landing Page

A single-page, mobile-first landing page that sends visitors to the official Toss King Ajay Telegram channel. The page shows the brand profile, highlight stats and features, and a 15-second countdown that redirects to Telegram on its own. It also has several "Join" buttons for visitors who don't want to wait.

## Technologies

- Plain HTML with no build step
- Tailwind CSS (Play CDN), Font Awesome icons and Google Fonts (Outfit, Rajdhani)
- A small inline script that runs the countdown and the redirect
- Hosted on Netlify (`netlify.toml` publishes the repository root)

## Running locally

Open `index.html` in a browser, or serve the folder with any static server:

```bash
netlify dev --port 8889
```

## Customizing

- **Telegram link:** change `targetTelegramUrl` in the script and the three `href="https://t.me/..."` links.
- **Countdown length:** change `totalSeconds`, and the starting `15` values in the markup.

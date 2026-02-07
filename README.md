# Collins Omwenga

Personal portfolio & rate card — Technical Consultant & Platform Engineer based in Nairobi, Kenya.

**Live:** [geekswagg.github.io](https://geekswagg.github.io)

## Features

- **Modern Dark Theme** — Clean, minimal design with CSS Grid
- **Rate Card** — Strategic Planning & IT Consulting, Business Consulting, Business Analytics & ALM
- **Skills Showcase** — Cloud Transformation, Kubernetes, Cybersecurity, Application Architecture, Business Development
- **Opportunities Section** — Consulting engagements, speaking & training, partnerships
- **Auto-Updating Forks Feed** — Daily GitHub Action fetches recent forks with Unsplash images

## Tech Stack

```
HTML5 + CSS3 (vanilla, no frameworks)
JavaScript (ES6+)
GitHub Actions (daily automation)
GitHub Pages (hosting)
```

## Project Structure

```
├── index.html              # Main portfolio page
├── forks.json              # Auto-generated forks data
├── scripts/
│   └── update-forks.js     # Fetches forks from GitHub API
├── .github/
│   └── workflows/
│       └── update-forks.yml  # Daily cron job
├── Resume/
│   └── COLLINS_OMWENGA_Resume.pdf
└── assets/                 # Legacy assets (CSS, JS, images)
```

## Auto-Updating Forks Feed

The site automatically updates daily with your latest forked repositories:

1. **GitHub Action** runs at midnight UTC
2. Fetches your most recent forks via GitHub API
3. Maps repo topics to relevant Unsplash images
4. Generates `forks.json` and commits to repo
5. Site renders cards from the JSON data

### Manual Trigger

```bash
gh workflow run update-forks.yml
```

## Local Development

```bash
# Clone
git clone https://github.com/geekswagg/geekswagg.github.io.git
cd geekswagg.github.io

# Serve locally
python -m http.server 8888

# Generate forks.json manually
node scripts/update-forks.js
```

## Rate Card

| Service | Rate |
|---------|------|
| Strategic Planning & IT Consulting | $80/hr |
| Business Consulting & Project Management | $100/hr |
| Business Analytics & ALM | $90/hr |

## Contact

- Email: comwenga@outlook.com
- LinkedIn: [collinsomwenga](https://linkedin.com/in/collinsomwenga)
- GitHub: [geekswagg](https://github.com/geekswagg)
- Twitter: [@omwenga_c](https://twitter.com/omwenga_c)

## License

MIT

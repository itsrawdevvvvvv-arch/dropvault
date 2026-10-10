# DropVault

Drop a file, get a shareable link. A tiny static uploader that commits your
files straight into this GitHub repo using the GitHub REST API — everything
runs in your browser, no server, no build step.

## The site

Open **https://itsrawdevvvvvv-arch.github.io/dropvault/** and drag files in.

- Uploaded files are committed to the `files/` folder of this repo.
- Each upload gives you a shareable link:
  `https://itsrawdevvvvvv-arch.github.io/dropvault/files/<name>`
- A CDN mirror is also offered:
  `https://cdn.jsdelivr.net/gh/itsrawdevvvvvv-arch/dropvault@main/files/<name>`

## One-time setup

The site uploads using your own GitHub account, so it needs a token:

1. Open the site and click **Create a token on GitHub**.
2. Generate it (the `public_repo` scope is pre-selected) and copy the value.
3. Paste it into the site and hit **Save & verify**.

The token is stored only in your browser's localStorage and is sent only to
`api.github.com`. You can revoke it any time from GitHub settings.

## Notes

- This repo is **public**, so every file you upload gets a public link.
  Do not upload private or sensitive documents.
- GitHub Pages takes ~1 minute to publish a freshly committed file.

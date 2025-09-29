# GameOfJones Static Site (GitHub Pages)
Public URLs for TikTok App Review.

## Live URLs (after Pages deploy)
- Terms: https://matthewod11-stack.github.io/GOJ/terms.html
- Privacy: https://matthewod11-stack.github.io/GOJ/privacy.html
- Reviewer: https://matthewod11-stack.github.io/GOJ/reviewer.html

## What to put into TikTok App Settings
- Terms URL → the Terms link above
- Privacy URL → the Privacy link above
- Redirect URI → use the Reviewer URL above **or** your backend callback
- Scopes: `video.publish`, `user.info.basic` (optionally `video.list`)

## Token Exchange (server-side)
POST https://open.tiktokapis.com/v2/oauth/token/
Content-Type: application/x-www-form-urlencoded
client_key=...&client_secret=...&code=...&grant_type=authorization_code&redirect_uri=...

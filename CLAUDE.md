# Working with this user

## X (Twitter) links

When the user shares an x.com / twitter.com link, read or watch it straight away. Never ask them to paste the content.

- Fetch `https://api.fxtwitter.com/<user>/status/<id>` (JSON: full text, media and video URLs, quoted post). This works from cloud sessions; the Default environment allows it.
- Opening x.com directly in the pre-installed headless Chromium returns 403 from X, so use the API above first and the browser only for media (`pbs.twimg.com`, `video.twimg.com`).
- If a host is refused by the network proxy, propose adding it to the environment instead of asking the user for the text.

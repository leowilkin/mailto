# mailto

A tiny static site that turns paths or query parameters into `mailto:` links.  
Deployed on [Vercel](https://vercel.com).

## Usage

Visit:

- `/leo` → opens `mailto:leo@hackclub.com`
- `/?to=alex&domain=example.com` → opens `mailto:alex@example.com`
- Add optional `subject` and `body` query params.

## Local development

Serve `index.html` locally:

```sh
python -m http.server 3000
# then open http://localhost:3000/?to=leo
```

For clean /leo style URLs locally, use the included Vercel dev server or a custom fallback server.

## Deployment

The project uses a vercel.json rewrite to always serve index.html.
Deploy with:

```
vercel --prod
```

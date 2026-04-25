# ForgeDITA Website

Static GitHub Pages website for ForgeDITA.

## Files

- `index.html`: home page
- `styles.css`: site styles
- `CNAME`: custom domain setting for `forgedita.com`
- `assets/`: logo concept and favicon

## GitHub Pages Setup

1. Create a GitHub repository for the site.
2. Add these files to the repository root.
3. In GitHub, go to **Settings > Pages**.
4. Set the source to deploy from the main branch root.
5. Set the custom domain to `forgedita.com`.
6. Enable **Enforce HTTPS** when GitHub allows it.

## DNS Setup

For the apex domain `forgedita.com`, create these A records with your DNS provider:

```text
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

For `www.forgedita.com`, create a CNAME record pointing to your GitHub Pages default domain, usually:

```text
<your-github-username>.github.io
```

Replace `<your-github-username>` with the actual GitHub user or organization name that owns the repository.

## Email Placeholder

The site uses `hello@forgedita.com` in mail links. Replace this address if needed before publishing.

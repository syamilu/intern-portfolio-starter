# Intern Portfolio Starter

A personal landing page with a blog, ready to deploy on Netlify's free plan. Write about your internship journey as Markdown files in `app/blog/posts/`.

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/syamilu/intern-portfolio-starter)

## Run it locally

```powershell
npm install
npm run dev
```

Open http://localhost:3000.

## What's different from the original

Based on Vercel's [Portfolio Starter Kit](https://github.com/vercel/examples/tree/main/solutions/blog) (commit `7770475`, 22 Apr 2026), MIT licence. Changed so it installs and runs on Netlify:

- `geist` bumped to `^1.8.1`. The pinned 1.2.2 doesn't install with Next.js 16.
- Vercel Analytics and Speed Insights removed.
- Blog post pages `await params`. Without it every post returned 404 on Next.js 15+.
- `baseUrl` reads Netlify's `URL` variable, so the sitemap, RSS and share images use your site's address.
- npm instead of pnpm.

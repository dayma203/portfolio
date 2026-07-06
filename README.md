# Dayton Massey — Portfolio Site

Setup guide and daily-use notes: see the full README in the project zip,
or the steps below.

## Stack

Astro static site + Decap CMS (admin at /admin), hosted on Netlify,
content stored in this repo.

## Daily use

Go to yoursite.netlify.app/admin, log in with GitHub, write, hit Publish.
The site rebuilds in about a minute.

- Hide a project: flip "Show on site" off in the admin and publish.
- Blog drafts never appear on the site.
- Export photos at ~2000px / under ~500 KB before uploading.

## Local development

```
npm install
npm run dev
```

## Admin login setup (one time)

1. GitHub → Settings → Developer settings → OAuth Apps → New OAuth App.
   Callback URL: https://api.netlify.com/auth/done
2. Netlify → Site configuration → Access & security → OAuth →
   Install provider → GitHub → paste Client ID and Secret.
3. Visit /admin and log in with GitHub.

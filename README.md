<img src="https://cdn.statically.io/gh/craigary/nobelium/main/Nobelium-Logo.svg" width="50" height="50">

# Nobelium

A static blog build on top of Notion and Nextjs, deployed on [Vercel](https://vercel.com?utm_source=Craigary&utm_campaign=oss).

<p>
  <a aria-label="GitHub commit activity" href="https://github.com/craigary/nobelium/commits/main" title="GitHub commit activity">
    <img src="https://img.shields.io/github/commit-activity/m/craigary/nobelium?style=for-the-badge">
  </a>
  <a aria-label="GitHub contributors" href="https://github.com/craigary/nobelium/graphs/contributors" title="GitHub contributors">
    <img src="https://img.shields.io/github/contributors/craigary/nobelium?color=orange&style=for-the-badge">
  </a>
  <a aria-label="Build status" href="#" title="Build status">
    <img src="https://img.shields.io/github/deployments/craigary/nobelium/Preview?logo=Vercel&style=for-the-badge">
  </a>
  <a aria-label="Powered by Vercel" href="https://vercel.com?utm_source=Craigary&utm_campaign=oss" title="Powered by Vercel">
    <img src="https://www.datocms-assets.com/31049/1618983297-powered-by-vercel.svg" height="28">
  </a>
</p>

Demo: [https://nobelium.vercel.app/](https://nobelium.vercel.app/)

<details><summary>Screenshot</summary>
<img src="https://github.com/craigary/nobelium/blob/main/desktop.png?raw=true">
</details>

## Highlights ✨

**🚀 &nbsp;Fast and responsive**

- Fast page render and responsive design
- Fast static generation with efficient compiler

**🤖 &nbsp;Deploy instantly**

- Deploy on Vercel in minutes
- Incremental regeneration and no need to redeploy after update the content in notion

**🚙 &nbsp;Fully functional**

- Comments, full width page, quick search and tag filter
- RSS, analytics, web vital... and much more

**🎨 &nbsp;Easy for customization**

- Rich config options, support English & Chinese interface
- Built with Tailwind CSS, easy for customization

**🕸 &nbsp;Pretty URLs and SEO friendly**

## Quick Start

- Star this repo 😉
- Duplicate [this Notion template](https://craigary.notion.site/ee99f65a23ab44f8ac80270122ee8138), and share it to the public
- [Fork](https://github.com/craigary/nobelium/fork) this project
- Customize `blog.config.js`
- _(Optional)_ Replace `favicon.svg`, and `favicon.ico` in `/public` folder with your own
- Deploy on [Vercel](https://vercel.com), set following environment variables：
  - `NOTION_PAGE_ID` (Required): The ID of the Notion page you previously shared to the web, usually has 32 digits after your workspace address
  - `NOTION_ACCESS_TOKEN` (Optional, not recommended): If you decide not to share your database, you can use token to let Nobelium grab data from Notion database. You can find it in your browser cookies called `token_v2`
    - Keep in mind Notion token is only valid for 180 days, make sure to update manually in vercel dashboard, we probably switch to Official API to resolve this issue in the future. Also, images in Notion database will not properly rendered
- **That's it!** Easy-peasy?

<details><summary>Wait for a sec, what is Page ID？</summary>
  <img src="https://github.com/craigary/nobelium/blob/main/pageid.png?raw=true">
</details>


## Roadmap

Check out our roadmap [here](https://craigary.notion.site/Public-Roadmap-89d184e51653445ab5b347e4efac079e)

- [x] Better SEO
- [x] Dark mode
- [x] Open Graph support
- [x] Switch to react-notion-x
- [x] Sitemap
- [ ] ...

## Technical details

- **Generation**: Next.js and Incremental Static Regeneration
- **Page render**: [react-notion-x](https://github.com/NotionX/react-notion-x)
- **Style**: Tailwind CSS and `@tailwindcss/jit` compiler
- **Comments**: Gitalk, Cusdis and more

## FAQ

<details>
  <summary>How can I change my avatar?</summary>
  Nobelium fetches avatars from <a href="https://gravatar.com">Gravatar</a>. You need to set your avatar there with <strong>the same email address</strong> that you defined in <code>blog.config.js</code>.
</details>
<details>
  <summary>My posts disappear after I set up grouping in Notion database!</summary>
  Nobelium currently doesn’t support Notion database grouping. If you really want to manage your posts by groups, you can create views with filters instead.
</details>


## License

The MIT License.

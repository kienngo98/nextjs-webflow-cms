# nextjs-webflow-cms
Create a blog with NextJS using Webflow API

A few things to keep in mind about Webflow API:
1. They use `undefined` instead of `null` on custom fields
2. They use hyphens for custom field name, somthing like `updated-on`
3. The API has low quota, so we need to implement a cache-solution when building the page (using getStaticPaths + getStaticProps)


Personal opinions:
1. I would use NextJS + Preact to reduce the JS bundle size
2. For 100% static pages, Astro is a really good option. However, my current project (the blog) has a filter/search feature so NextJS is a better choice.

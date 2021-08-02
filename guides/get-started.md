---
id: get-started
title: Getting started
---

[get-started]: https://www.flyyer.io/get-started
[new-project]: https://www.flyyer.io/dashboard/_/projects/new
[current-project]: https://www.flyyer.io/dashboard/_/projects
[guides-with-full-examples]: #guides-with-full-examples

## Install Flyyer previews

### 1. Create a project

A project is created when you synchronize a website with Flyyer.

* If you already have an account **[create a project here][new-project].**
* If you are a new user **[click here to get started][get-started].**

### 2. Insert smart image URLs in your meta-tags

It's built with your **project identifier** and the current `pathname` of your site which lets our system enrich your preview automatically. [Find your project identifier here](https://flyyer.io/dashboard/_/projects/_/integrate?ref=docs).

In HTML it would look like this:

```html
<meta property="og:image" content="https://cdn.flyyer.io/v2/{project-identifier}/_/_/{path}" />
<meta name="twitter:image" content="https://cdn.flyyer.io/v2/{project-identifier}/_/_/{path}" />
<meta name="twitter:card" content="summary_large_image" />

<!-- [Recommended] Keep your original image handy for your project -->
<meta property="flyyer:default" content="{your-original-og:image-link}" />
```

To see a **full example** please [select your website technology or programming language][guides-with-full-examples].

### 3. Voilà 🎉

Now you're able to manage your link previews from your dashboard, create content from templates while preserving your brand style and export it as social media formats.

[Go to your dashboard 🚀](https://flyyer.io/dashboard/_/projects/_/)

## Guides with full examples

### JavaScript guides

* [JavaScript and TypeScript](/guides/javascript/flyyer-js)
* [Next.js](/guides/javascript/nextjs)
* [Gatsby.js](/guides/javascript/gatsbyjs)
* [Express.js](/guides/javascript/expressjs)
* [Docusaurus.io](/guides/javascript/docusaurus)

### Python guides

* [Python](/guides/python/flyyer)
* [Django](/guides/python/django)

### Ruby guides

* [Ruby](/guides/ruby/flyyer)
* [Ruby on Rails](/guides/ruby/rails)

### PHP guides

* [PHP](/guides/php/flyyer)
* [Wordpress](/guides/php/wordpress)

---

Are we missing an integration guide? Need help? **Feel free to join our [Discord Channel](https://www.flyyer.io/discord).**

# WSWhitehouse.github.io - Personal Website & Blog.

This website is powered by [Jekyll](https://jekyllrb.com/) using a custom theme called [Chirpy](https://github.com/cotes2020/jekyll-theme-chirpy) and is hosted using GitHub pages.

## Building & Publishing The Site
The website is automatically built using a [GitHub Action](https://github.com/WSWhitehouse/WSWhitehouse.github.io/actions/workflows/build.yml) on every push to the `main` branch. This Action sets up the correct environment and prerequisites, builds the Jekyll site and pushes the updated site to the `gh-pages` branch. The `gh-pages` branch is set up as the site source so any changes will be updated to the live website. Checking out the `gh-pages` branch will show the live website - although, no manual changes should be submitted as they may be overwritten by the GitHub Action.

## Writing A New Post
Create a new file named `YYYY-MM-DD-TITLE.md` and put it in the `_posts/` folder in the root directory.

You need to fill the [Front Matter](https://jekyllrb.com/docs/front-matter/) as below at the top of the file:
```
---
title: TITLE
date: YYYY-MM-DD HH:MM:SS +/-TTTT
categories: [TOP_CATEGORY, SUB_CATEGORY] # Only two elements
tags: [TAG] # TAG names should always be lowercase, number of elements can range from zero to infinity
---
```

For more details check out the [Chirpy wiki page on writing a new post](https://github.com/cotes2020/jekyll-theme-chirpy/wiki/Writing-a-New-Post).

## Adding A New Tab
The website contains multiple tabs that can be seen in the left panel. These are controlled by markdown files located in the `_tabs/` folder in the root of this repository. The tabs `categories`, `tags`, and `archives` are special tabs and should not be removed or have any text (apart from the Front Matter) written in them.

Create a new file named `TITLE.md` and put it in the `_tabs/` folder in the root directory.

You need to fill the [Front Matter](https://jekyllrb.com/docs/front-matter/) as below at the top of the file:
```
---
title: TITLE
icon: fas ICON # Check out `Jekyll Font Awesome Icons` in the Useful Links section below
order: ORDER # Order in left panel
---
```

Additional content can be added to the tab page by adding it below the front matter.

## Useful Links
- Jekyll - [https://jekyllrb.com/](https://jekyllrb.com/)
- Jekyll Font Awesome Icons - [https://aksakalli.github.io/jekyll-doc-theme/docs/font-awesome/](https://aksakalli.github.io/jekyll-doc-theme/docs/font-awesome/)
- Chirpy Theme - [https://github.com/cotes2020/jekyll-theme-chirpy](https://github.com/cotes2020/jekyll-theme-chirpy)
- Chirpy Wiki - [https://github.com/cotes2020/jekyll-theme-chirpy/wiki](https://github.com/cotes2020/jekyll-theme-chirpy/wiki)
- Chirpy Starter Repo - [https://github.com/cotes2020/chirpy-starter](https://github.com/cotes2020/chirpy-starter)
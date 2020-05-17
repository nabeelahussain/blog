# Gatsby + Netlify CMS Blog

[![Netlify Status](https://api.netlify.com/api/v1/badges/b654c94e-08a6-4b79-b443-7837581b1d8d/deploy-status)](https://app.netlify.com/sites/gatsby-starter-netlify-cms-ci/deploys)

This repo contains my blog that is built with [Gatsby](https://www.gatsbyjs.org/), and [Netlify CMS](https://www.netlifycms.org): **[Live Link](https://www.nabs.dev/)**.

It follows the [JAMstack architecture](https://jamstack.org) by using Git as a single source of truth, and [Netlify](https://www.netlify.com) for continuous deployment, and CDN distribution.

## Features

- A simple landing page with blog functionality built with Netlify CMS
- Editabe Pages: Landing, Artwork, Blog and Contact page with Netlify Form support
- Create Blog posts from Netlify CMS
- Tags: Separate page for posts under each tag
- Uses Bulma for styling, but size is reduced by `purge-css-plugin`
- Fast loading times thanks to pre-rendered HTML and automatic chunk loading of JS files
- Uses `gatsby-image` with Netlify-CMS preview support
- Separate components for everything
- Netlify deploy configuration
- Netlify function support, see `lambda` folder
- Perfect score on Lighthouse for SEO, and very good for Accessibility and Performance

## Prerequisites

- [Node](https://nodejs.org/)
- [Gatsby CLI](https://www.gatsbyjs.org/docs/)
- [Netlify CLI](https://github.com/netlify/cli)

## Deploy your own!

Use the button below to build and deploy your own copy of the repository:

<a href="https://app.netlify.com/start/deploy?repository=https://github.com/nabeelahussain/blog&amp;stack=cms"><img src="https://www.netlify.com/img/deploy/button.svg" alt="Deploy to Netlify"></a>

After clicking that button, you’ll authenticate with GitHub and choose a repository name. Netlify will then automatically create a repository in your GitHub account with a copy of the files from this repo. Next, it will build and deploy the new site on Netlify, bringing you to the site dashboard when the build is complete. Next, you’ll need to set up Netlify’s Identity service to authorize users to log in to the CMS.

## Purgecss

This plugin uses [gatsby-plugin-purgecss](https://www.gatsbyjs.org/packages/gatsby-plugin-purgecss/) and [bulma](https://bulma.io/). The bulma builds are usually ~170K but reduced 90% by purgecss.

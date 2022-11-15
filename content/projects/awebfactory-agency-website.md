---
title: AWebFactory agency website
description:
  "AWebFactory.com: Migration from Drupal and WordPress to a decoupled
  Javascript web app"
date: 2022-11-08T10:39:34.459Z
startDate: 2022-11-08T10:39:34.458Z
endDate: ""
preview: ""
draft: true
mvp: mvp02
status: in planning
repo: ""
labels: ""
tags: ""
categories: ""
type: project
slug: awebfactory-agency-website
---

We've tried migrating multiple ways:

- headless wordpress plus react front end
- headless cms (directus, payload, strapi) plus react or vue based front end
- a content and content modeling first local markdown file based react or vue based front end
- final candidates:
  - Next 13 + Contentlayer
  - Nuxt 3 + Nuxt Content Module + Front Matter CMS
- and the winner (developed as a web app via the [Project Flow & Tracker project](/projects/project-flow-tracker)) has been:
  - Nuxt 3 + Nuxt Content Module + Front Matter CMS hosted on Netlify

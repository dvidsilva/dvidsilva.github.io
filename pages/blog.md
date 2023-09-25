---
name: Blog
nav: true
title: Blog | Daveed
description: Thoughts and stories
layout: full
permalink: '/posts'
---

## Blog Posts

{{#blog_posts files}}
- [{{item.attrs.title}}]({{item.attrs.permalink}})
{{/blog_posts}}

### Footer

[Home](/)

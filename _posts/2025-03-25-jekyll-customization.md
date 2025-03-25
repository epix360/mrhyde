---
title: "Customizing Your Jekyll Blog"
author: "John Doe"
date: "2025-03-25 16:32:55 -0600"
categories: tutorial
---

# Customizing Your Jekyll Blog

Jekyll offers numerous ways to customize your blog to match your style and needs. Here's a guide to some essential customization options.

## Theme Customization

The default Minima theme provides a great starting point, but you can easily modify it:

```scss
// Add to assets/css/main.scss
$brand-color: #2a7ae2;
$text-color: #333;
$background-color: #fdfdfd;

body {
  font-family: 'Helvetica Neue', Arial, sans-serif;
  line-height: 1.6;
}
```

## Layout Options

You can create custom layouts in the `_layouts` directory:

```html
<!-- Example of a custom layout -->
{% raw %}
<article class="post">
  <header class="post-header">
    <h1>{{ page.title }}</h1>
    <time>{{ page.date | date: "%B %d, %Y" }}</time>
  </header>
  
  {{ content }}
</article>
{% endraw %}
```

## Adding Features

Some popular features you might want to add:

1. **Comments System**
   - Disqus
   - Utterances (GitHub-based)
   - Giscus

2. **Analytics**
   - Google Analytics
   - Plausible
   - Simple Analytics

3. **Social Sharing**
   - Twitter/X
   - LinkedIn
   - Facebook

## Next Steps

In the next post, we'll explore advanced Jekyll features like collections, data files, and custom plugins.

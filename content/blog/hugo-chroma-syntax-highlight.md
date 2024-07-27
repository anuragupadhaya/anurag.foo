+++
author = "Anurag Upadhaya"
title = "Change Chroma syntax highlight in Hugo"
date = "2024-07-27"
description = "Change Chroma syntax highlight in Hugo"
tags = [
    "hugo",
    "TIL",
]
+++

You can explore all the Chroma themes at [Chroma Playground](https://swapoff.org/chroma/playground/)

### To change Chroma syntax highlighting for your theme:

1. Make Hugo use classes instead of inline styles

```toml
[markup]
  [markup.highlight]
    noclasses = false
```

2. Generate new Chroma stylesheets

```bash
hugo gen chromastyles --style=monokai > layouts/partials/css/syntax-dark.css
```

Based on your theme, you can either have this new stylesheet load through `<link>` or through css media queries.

<small>Sources:</small>

https://aamnah.com/notes/hugo/hugo-custom-chroma-syntax-highlighting/
https://bwiggs.com/posts/2021-08-03-hugo-syntax-highlight-dark-light/

+++
title = "Markdown & metadata"
weight = 3
+++

In **Infusion**, design patterns are documented using markdown. To create a new pattern file, just add a file with the `.md` extension to the `/patterns` folder. It's recommended you use "kebab case" to name the file ( words separated by hyphens). For example, a pattern with the title "Menu button" should probably have the filename `menu-button`. Then you get a nice clean URL: `your-company.com/patterns/menu-button`.

If you're not familiar with writing markdown, there are a number of tutorials available. One of the best is [Mastering Markdown](https://guides.github.com/features/mastering-markdown/) offered by Github. There's also a [nice cheatsheet here](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet).

## The metadata

Like many static site generators, Hugo lets you add metadata to its markdown files. Hugo's brand of metadata is called TOML (although YAML is also accepted). The only thing you _have_ to put in the TOML is a `title` — like this:

```
+++
title = "Menu button"
+++
```

### Tags

If you like, you can also tag the pattern so that it turns up in lists of similar content. You add tags in an array format. Note that all the TOML data is found at the top of the markdown file, between the `+++` lines.

```
+++
title = "Menu button"
tags = ["interactive", "popup", "javascript"]
+++
```

This will create links to tag pages listing content tagged with the same terms.
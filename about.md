---
layout: page
title: Jekyll
permalink: /about/
---
:cn:

* [jekyll](https://jekyllrb.com/)
* [cheat sheet](https://learn.cloudcannon.com/jekyll-cheat-sheet/)
* [prism](https://prismjs.com/)
* [isotope](https://isotope.metafizzy.co/)
* [Modular Scale](https://www.modularscale.com/)
* [yaml](https://yaml.org/)
* [liquid](https://liquid.bootcss.com/)
* [parceljs](https://www.parceljs.cn/)
^
markdown :+1:

* [kramdown quick](https://kramdown.gettalong.org/quickref.html)
* [kramdown syntax](https://kramdown.gettalong.org/syntax.html)
* [gfm](https://github.github.com/gfm/) :heart:
* [commonmark](https://daringfireball.net/projects/markdown/)
* [github emoji](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md#smileys--emotion)
^
plugs
* [jekyll-target-blank](https://github.com/keithmifsud/jekyll-target-blank)
* [jemoji](https://github.com/jekyll/jemoji)

## setup

```sh
gem install jekyll bundler
jekyll new myblog
```

## liquid

* objects
* tags
* filters

## front matter

```yaml
---
title: Home
---
```

## layouts

```yaml
---
layout: default
title: Home
---
```

## includes

目录：_includes

<!-- {% raw %} -->
```liquid
{% include navigation.html %}
```
<!-- {% endraw %} -->

## data

目录：_data

```yaml
# _data/navigation.yml
- name: Home
  link: /
- name: About
  link: /about.html
```

<!-- {% raw %} -->
```liquid
<nav>
  {% for item in site.data.navigation %}
    
  {% endfor %}
</nav>
```
<!-- {% endraw %} -->

## Aserts

## theme

```sh
bundle info --path minima

```

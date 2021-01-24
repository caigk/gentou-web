---
layout: page
title: About
permalink: /about/
---

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

```template
{ % include navigation.html % }
```

## data

目录：_data

```yaml
# _data/navigation.yml
- name: Home
  link: /
- name: About
  link: /about.html
```

```template
<nav>
  { % for item in site.data.navigation % }
    
  { % endfor % }
</nav>
```

## Aserts


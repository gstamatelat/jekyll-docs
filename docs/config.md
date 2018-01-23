---
layout: page
title: Configuration
permalink: /config/
---

Create a `_config.yml` in the root of the site directory.

```yaml
remote_theme: gstamatelat/jekyll-docs@{{site.version}}
baseurl: BASE_URL
title: SITE_TITLE
menu: MENU_ITEMS
links: LINKS
```

##### `BASE_URL`

The base URL of your site.

Must not have a trailing slash. Must begin with slash.

For example if your site is hosted on
`https://my_username.github.io/my_project/`, use
```yaml
baseurl: /my_project
```

##### `SITE_TITLE`

The title of your site.

This will be visible in the navbar of the site.

For example
```yaml
title: MyPackage documentation
```

##### `MENU_ITEMS`

The contents of the sidebar.

You can define a sequence of groups, where each group contains a sequence of
URLs. A page must exist for each URL. The layout will automatically pick up the
title of the page and set it as the label for the menu item.

For example

```yaml
menu:
  Start here:
    - /
    - /getting-started/
  Second menu:
    - /import/
```

will create a sidebar of two menu groups with labels `Start here` and `Second
menu` respectively. Three pages must exist in the site, with the attribute
`permalink` set to `/`, `/getting-started/` and `/import/`.

##### `LINKS`

The links in the navbar.

A map of links, where keys are the font awesome icon code and the value is the
link target.

For example

```yaml
links:
  github: https://github.com/my_username/my_project
  twitter: https://twitter.com/my_username
```

---
layout: page
title: Pages
permalink: /pages/
---

Pages in the site must have at least the following front matter:

```yaml
layout: page
title: PAGE_TITLE
permalink: PERMA_LINK
```

##### `PAGE_TITLE`

This attribute will define the label of the menu item in the sidebar (if the
page is configured in the menu) as well as the header of the page when
displayed.

##### `PERMA_LINK`

This attribute value must match the value set in `MENU_ITEMS`.

For example if you have the following (partial) `menu` setup:

```yaml
menu:
  Menu label:
    - /first-item/
```

the `permalink` attribute of the respective page must be

```yaml
permalink: /first-item/
```

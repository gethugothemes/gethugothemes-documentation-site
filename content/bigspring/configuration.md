---
title: "Configuration"
date: 2020-12-23T10:00:00+07:00
weight: 2
---

In your sites root folder you will find a file called `config.toml`. Open this file with your text editor or IDE.

## Sitewide configuration

{{< contentblocklist "configsidewide/" "baseURL" "summaryLength" "theme" "title" "googleAnalytics" "disqusShortname" >}}

## Plugin Configuration

You can add third party plugins from here very easily, We create a loop for plugins, you will see two plugins loop here, first one is for `css` and last one is for `js`. just copy a loop item that you need and paste it in the bottom of the loop. and link correctly, after added a plugins, you maybe need to close the hugo server and run it again for rendered correctly.

## Menu Configuration

* `[[menu.main]]` is the main menu loop, you can add your navigation item by copy and pasting this line.
* `name` attribute is for navigation item name.
* `URL` is for the page url, just give the page name here, it will automatically add the base URL from your site. like if you want to give the about page url here, just type `about` .
* `weight` is for your navigation sorting, the smaller number weight will show first.

```toml
[[menu.main]]
weight = 5
name = "Pages"
hasChildren = true
```

This theme comes with four configurable menus:

```toml
[[menu.main]]
[[menu.footer_left]]
[[menu.footer_middle]]
[[menu.footer_right]]
```

## Parameter Configuration

Most parameters in the `[params]` section of your configuration are commented. You can change the basic setup of the theme and add information or enable/disable features.

## Homepage Configuration

You can configure all elements on the homepage by changing the values in `data/homepage.yml`. To hide any element set `enable` to false in the corresponding section. 

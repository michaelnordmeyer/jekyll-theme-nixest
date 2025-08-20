# Jekyll Theme Nixest

The even more barebones cousin of the barebones themes [“Nix”](https://github.com/michaelnordmeyer/jekyll-theme-nix) and [“Nixer”](https://github.com/michaelnordmeyer/jekyll-theme-nixer) for [Jekyll](https://github.com/jekyll/jekyll). It is optimized for fast build speeds as well.

Its purpose is to be a hard-core minimalist, single-author theme while not displaying anything more than just the content of posts and a list of posts.

It also changes as little as possible from the default browser settings to improve legibility.

[Demo](https://jekyll-theme-nixest.michaelnordmeyer.com/)

![Screenshot](/screenshot.png)

It is meant for people, who are aware that nobody is using RSS feeds anymore. Either because they don't know what they are or how to use them, or they replaced Google Reader with Social Media. So all visitors are coming from search engines – let's be honest, Google – and won't read other posts, unless they are linked in the post itself.

And people coming from hacker news or related sites know how to change the URL in the browser's address bar.

This is an open-an-editor-an-just-start-writing theme. Compared to [“Nixer”](https://github.com/michaelnordmeyer/jekyll-theme-nixer), which has title support, “Nixest” doesn't show any, but only the first 150 characters of a post in places where titles normally are displayed. This means the beginning of posts should use those characters for something reasonable like a summary or introduction and shouldn't have any titles. It's up to the writer to make this approach work.

If you think this goes too far, use the above mentioned [Jekyll theme “Nix”](https://github.com/michaelnordmeyer/jekyll-theme-nix) instead.

[I wrote up what inspired me to create the three themes](https://michaelnordmeyer.com/i-created-three-ultra-minimalistic-jekyll-themes).

## Limited Features

- Dark mode, because we want to be respectful
- Posts, but no backlink to homepage
- No Pages, except custom error pages
- No visible titles, dates, authors, categories, or tags on posts and pages
- No header or footer
- No pagination for the home page
- No feeds
- A sitemap.xml, because search engines should index us properly
- No semantic info like Open Graph, Twitter cards, JSON-LD, or Microdata

## Minutiae

### Default Colors

The default colors are the colors of the respective browsers, both in light and in dark mode.

### Favicon

`/assets/icons/icon.webp` is the favicon for the light mode, and there's also a dark variant `/assets/icons/icon-dark.webp` for dark mode. They will be used automatically or you can replace them by creating new ones in the same location.

### Nixest?

“Nix” is the grammatically incorrect form of the German “nichts”, which in English means “nothing”. It's colloquially used to stress the nothingness. “Nixer” is the even more grammatically incorrect comparative of that, which colloquially may or may not being used at all. And “Nixest” is the Englisch superlative of “Nix”.

Or, if you will, it could be UNIX without the “U”, because of the theme's somewhat archaic properties, but even more archaic.

## Installation

Installation from Gem is recommended, but using a remote theme is also possible, even though it will increase build times a little, depending on your internet connection and the size of the theme download, because it will be downloaded during each build. Gems are installed locally.

GitHub Pages gem users need to use the remote theme method.

### Installation from Gem

Add this line to your Jekyll site's `Gemfile`:

```ruby
gem "jekyll-theme-nixest", group: [:jekyll_plugins]
```

Then run `bundle` in your terminal.

```sh
bundle
```

Also add the theme to your Jekyll site's `_config.yml`:

```yaml
theme: jekyll-theme-nixest
```

Make sure that this is the only `theme:` in `_config.yml`, and that there are no other `remote-theme:`.

### Installation as Remote Theme

Add this line to your Jekyll site's `Gemfile`:

```ruby
gem "jekyll-remote-theme", group: [:jekyll_plugins]
```

Then run `bundle` in your terminal.

```sh
bundle
```

Finally add the remote theme to your Jekyll site's `_config.yml`:

```yaml
remote_theme: michaelnordmeyer/jekyll-theme-nixest
```

Make sure that this is the only `remote_theme:` in `_config.yml`, and that there are no other `theme:`.

# Webseite des Asozialen Netzwerkes

## How to run the website locally
Make sure you have [RubyGems](https://rubygems.org/) installed.
```
gem install bundler jekyll
git clone https://github.com/asozialesnetzwerk/asozialesnetzwerk.github.io.git
cd asozialesnetzwerk.github.io
bundle exec jekyll serve
```

## How to edit wiki articles
Wiki articles are located in the `_wiki` folder.
They are using simple markdown, which should make it fairly easy to modify them.

## How to create wiki articles
A wiki article has the following structure:
```
---
title: "Article title"
headline: "Article headline"
position: 3
keywords:
- keyword1
- keyword2
---

The content of the article.
```
* `title`: The title of the article, which will be used for the `<title>` html tag and the side navigation
* `headline`: The headline of the article, displayed as `<h1>`. If not set, the title is used.
* `position`: The position of the article in its category. Starting with `1`.
* `keywords`: A list with keywords used for search. Don't repeat the title or headline here.

## How to create changelogs
Changelogs are located in the `_changelog` folder. They have the following structure:
```
---
title: "Version x.y.z"
version: x.y.z
---

The content of the changelog.
```
* `title`: The title of the changelog, which will be used for the `<title>` html tag, usually `Version :version:`
* `version`: The version number
## Getting Started

You can use [Prose.io](http://prose.io/#opennorth/opennorth.ca/) to edit the website. Otherwise:

```
gem install bundler
git clone git@github.com:opennorth/opennorth.ca.git
cd opennorth.ca
bundle
```

## Making Changes

To **add a news item**, create a file in the `_posts` folder with a name following the pattern `YYYY-MM-DD-descriptive-filename.html` and with contents of:

```yaml
---
categories: news
title: A descriptive sentence
url: A URL including http://
---
```

To **edit the staff or board**, edit the `_data/staff.yml` and `_data/board.yml` files.

## Preview Changes

Before committing your changes, always preview your changes. Start a server with `bundle exec jekyll serve -w` and open [0.0.0.0:4000](http://0.0.0.0:4000) in a browser. While the server is running, you can make changes to files, then refresh the page in the browser to see your changes immediately! Press `Ctrl+C` to stop the server.

*Note:* This command compiles HTML files into the `_site` directory. Do not edit those files. Your changes to those files will not be saved.

*Note:* If the server is running, you must issue commands in a different Terminal window. Typing commands in the Terminal window in which the server is running will have no effect.

## Theme

These files should be identical in this repository and [nordouvert.ca](https://github.com/opennorth/nordouvert.ca/):

* `.gitignore`
* `.gitmodules`
* `_config.yml`
* `dir.ttl`
* `Gemfile`
* `Gemfile.lock`

In other words, only these files should differ:

* `_data/`
* `_posts/`
* `community/`
* `communaute/`
* `CNAME`
* `index.html`

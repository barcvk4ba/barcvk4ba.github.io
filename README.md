![Nightly Rebuild](https://github.com/barcvk4ba/barcvk4ba.github.io/workflows/Nightly%20Rebuild/badge.svg)

# Brisbane Amateur Radio Club

This is a web site for BARC.

It uses [Jekyll](https://jekyllrb.com/docs) for site generation and is hosted by GitHub.


# Theme Details

We are currently using the [minimal
mistakes](https://mmistakes.github.io/minimal-mistakes) and this has some good
documentation on how to configure and customise.

We use:
* `pages` for main navigation items
* `posts` for aritcles, updates and things happening
* and various collections for other useful documents

# How to edit on your computer

This is best done on a Linux computer, although they claim Windows is possible,
we haven't tried.

## Setting Up

1. Install Ruby. [Installation Guide](https://jekyllrb.com/docs/installation/)
   This document assumes you are installing on a Linux System, but it may be
   possible under Windows.
2. Install the Rugy Gem `bundler`
   ```
   gem install bundler
   ```
3. Clone this repository. You will have to put it somewhere, I'd suggest
   `~/Git`.
   ```
   cd ~/Git
   git clone git@github.com:barcvk4ba/barcvk4ba.github.io.git
   ```
4. Go into the repository and run the initial set up to install the required
   tools to build and run the site locally
   ```
   cd ~/Git/barcvk4ba.github.io
   bundle install
   ```

As you are editing the site, be sure to run `bundle update` regularly to keep
Jekyll and the GitHub tools up to date.

## Building / Serving the Site Locally

Once set up, you can run jekyl locally, serving the content as you edit by running the
`serve.sh` script in the root of this repo.

```
cd ~/Git/barcvk4ba.github.io
./serve.sh
```

This will compile the site and start serving it on the local computer port, 4000.
This script is set up to bind to all IP addresses on the machine, may not
be what you want, feel free to adjust the script, but don't commit those
changes.

You should now be able to navigate to `http://127.0.0.1:4000` and see the site.

## Making Changes

In most cases, you are likely to be adding content, rather than messing with
settings, so all you need to do is add a Markdown file in the right place.

* `_posts` contains news items. These must be named with no spaces in the form
  `YYYY-MM-DD-some-meaninful-name.md`
* `_articles` contain articles. I suggest they follow the same naming
  convention as posts.
* `_projects` contain projects. I suggest they follow the same naming
  convention as posts.

Each file must have some _Front Matter_ defined that tells Jekyll what to do
with the file. I've set up sensible defaults for this, but you have to provide
at a minimum the title and date.

Front matter is in YAML format and must be the first lines of the file.

```
---
# This is front matter (this is a comment)
title: A Title For you document
date: 2020-05-17 19:30:00 +1000
---

This is the first line of content...
```

You should read about Markdown and YAML, but see what is there and copy should
get you a long way.

## Committing Changes and Publishing

This is a git repository. You will need to add the changes you have made to the
index, them commit it with a suitable message describing what was done.

Once you've done that, it is stored locally and you need to push it to GitHub.

NOTE: This is a bit topic in itself. Perhaps look at the Github documentation.

## Editing on GitHub

If all you are doing is adding a new post, article or project Markdown file, it
is possible to edit this directly on GitHub using the `Create New File` button
(making sure you're in the right folder first).

You can also edit an existing file by clicking on it, then Edit (Pencil) icon.

You will have to fill in a commit message like you would do locally before you
can complete the add/edit.








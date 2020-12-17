---
title: "Cara Install Python di Laptop"
date: 2020-12-09
slug: cara-install-python
description: "A quick read on how to get started with Hugo."

tags:
- python
categories:
- Programming
- tutorial

draft: false

featured_image : https://1.bp.blogspot.com/-Nb-2ANb8_zw/X9JZi6_fQuI/AAAAAAAAABY/5WIZyA0W5h0wRhngwunTq09YJLOGgQZBwCNcBGAsYHQ/s16000/default.png
cover_image: https://1.bp.blogspot.com/-TvkeU85rpLY/X9uL6cQ4AqI/AAAAAAAAAWk/R8013QgjZcIP0akYc1bR_2uSWAZbSoHrQCLcBGAsYHQ/s16000/cover.png
---

# Step 1. Install Hugo

Goto [hugo releases](https://github.com/spf13/hugo/releases) and download the
appropriate version for your os and architecture.

Save it somewhere specific as we will be using it in the next step.

More complete instructions are available at [installing hugo](/overview/installing/)

# Step 2. Build the Docs

Hugo has its own example site which happens to also be the documentation site
you are reading right now.

Follow the following steps:

 1. Clone the [hugo repository](http://github.com/spf13/hugo)
 2. Go into the repo
 3. Run hugo in server mode and build the docs
 4. Open your browser to http://localhost:1313

Corresponding pseudo commands:

```bash
git clone https://github.com/spf13/hugo
cd hugo
/path/to/where/you/installed/hugo server --source=./docs
> 29 pages created
> 0 tags index created
> in 27 ms
> Web Server is available at http://localhost:1313
> Press ctrl+c to stop
```

Once you've gotten here, follow along the rest of this page on your local build.

# Step 3. Change the docs site

Stop the Hugo process by hitting ctrl+c.

Now we are going to run hugo again, but this time with hugo in watch mode.

```bash
/path/to/hugo/from/step/1/hugo server --source=./docs --watch
> 29 pages created
> 0 tags index created
> in 27 ms
> Web Server is available at http://localhost:1313
> Watching for changes in /Users/spf13/Code/hugo/docs/content
> Press ctrl+c to stop
```


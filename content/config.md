+++
title = "Configuration"
weight = 1
+++
The site can be configured in the file `Blades.toml` in its root directory. There, the following
variables can be set. All of them are optional, default values are shown.

**Any** other variable of **any type** can be set there and used in the templates, too.

```toml
# Title of the site
title = ""
# URL which the site is expected to be accessed through
url = ""
# Name of the folder where theme templates and assets shall be loaded from,
# located in the themes directory (see below)
theme = ""
description = "" 
keywords = ""
image = ""

# Generate sitemap
sitemap = true
# Generate RSS feed
rss = true
# Generate Atom feed
atom = true
# Generate taxonomies that were not explicitly defined in this config
implicit_taxonomies = true
# When no date for a page is specified, use the file creation date
dates_of_creation = true

# A directory where the content is loaded from
content_dir = "content"
# A directory where the theme is loaded from
theme_dir = "themes"
# A directory where the content is rendered to
output_dir = "public"
# A subdirectory of the output directory where the assets are copied to
assets = "assets"

[author]
name = ""
uri = ""
email = ""
avatar = ""

# A table of tables where you can specify some data about taxonomies
[taxonomies]
# Example with default values:
tags = { name = "", description = "", template = "taxonomy.html", key_template = "taxonomy_key.html", paginate_by = inf, sort_by_weight = false }
# If provided, 'paginate_by' must be a positive integer
```
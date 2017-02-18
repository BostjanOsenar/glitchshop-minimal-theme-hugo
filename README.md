# glitchshop-minimal-theme-hugo

A minimal theme for Hugo created using Bootstrap v4 alpha 6.
It is designed to use externally hosted CSS and Javascript libraries and minimal custom CSS to add formatting touches where needed while providing basic blog functionality.

## Configuration details
Below is an example of TOML front matter that includes description, categories and tags used with this theme:
~~~
+++
date = "2017-12-02T23:18:50Z"
draft = false
title = "Plain vanilla theme for Hugo"
description = "A simple starter theme for Hugo made with Bootstrap 4 alpha 6"
author = "Bostjan"
categories = [ "Static Website"]
tags = [ "Hugo", "Bootstrap" ]
featured = "/media/content/hugo-bootstrap-minimal-theme-feature.jpg"
+++

...
~~~

A sample configuration file (_config.toml_):
~~~
languageCode = "en-us"
baseurl = "http://glitchshop.com/"
theme = "glitchshop-minimal-theme"
title = "Glitchshop"
copyright = "Copyright © 2016-2017 Bostjan Osenar. All rights reserved."
pluralizeListTitles = false
paginate = 18

[permalinks]
  post = "/:year/:month/:title/"

SectionPagesMenu = "main"
[[menu.main]]
  name = "Home"
  identifier = "home"
  url = "/"
  weight = 0
[[menu.main]]
  name = "Projects"
  identifier = "projects"
  url = "/projects/"
  weight = 1
[[menu.main]]
  name = "Blog"
  identifier = "blog"
  url = "/blog/"
  weight = 2

[params]
  logo = "media/branding/glitchshop-white-lg.png"
[params.home]
  postsSection = "blog"
  postsSectionLink = "/blog/"
  projectsSection = "projects"
[params.social]
  linkedin = "https://www.linkedin.com/in/bosenar"
  github = "https://github.com/BostjanOsenar"

[taxonomies]
  category = "categories"
  tag = "tags"
~~~

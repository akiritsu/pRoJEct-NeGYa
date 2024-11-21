
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]

<!-- LOGO -->
<br />

<p align="center">
  <a href="https://github.com/akiritsu/pRoJEct-NeGYa">
    <img src="src/assets/img/favicon.png" alt="Logo" width="80" height="80">
  </a>

  <h3 align="center">pRoJEct-NeGYa</h3>
    <h5 align="center">v 3.0</h5>
    <br />
  <p align="center">
    pRoJEct-NeGYa is a hacker-like, highly-customizable theme for note-keeping, personal-website or CV.
    <br />
    <br />
    <a href="https://akiritsu.github.io/pRoJEct-NeGYa/">View Demo</a>
    ·
    <a href="https://github.com/akiritsu/pRoJEct-NeGYa/issues">Report Bug</a>
    ·
    <a href="https://github.com/akiritsu/pRoJEct-NeGYa/issues">Request Feature</a>
  </p>

</p>

<!-- TABLE OF CONTENTS -->
## Table of Contents

* [Table of Contents](#table-of-contents)
* [About The Project](#about-the-project)
  * [Features](#features)
  * [Builtwith](#builtwith)
* [Getting Started](#getting-started)
  * [Prerequisites](#prerequisites)
  * [Installation](#installation)
  * [Personalize and Customize](#personalize-and-customize)
    * [\_config.yml](#_configyml)
    * [Collections](#collections)
    * [Writing](#writing)
    * [Comment](#comment)
    * [Test locally](#test-locally)
    * [Front Matter](#front-matter)
* [Roadmap](#roadmap)
* [Contributing](#contributing)
* [License](#license)
* [Contact](#contact)


<!-- ABOUT THE PROJECT -->
## About The Project

![homepage]({{site.img}}/Screenshot-2.png)

This jekyll theme is a content-oriented blog, cv or learning notes, aimed at providing a convinient note-keeping tool. You can keep and review your notes or articles in different collections without any functional recode.

### Features

* Highly customizable
* Formula insertion
* Code test online
* Easy-to-use cheatsheet
* Hacker-like theme
* Code highlight
* Text Decryption
* Convinient code exhibition and review
* Table of content
* Atom Feeds
* SEO

### Builtwith

* Bundler
* Jekyll
* Mathjax
* Font Awesome
* Sjcl
* Disqus
* Mermaid

## Getting Started

### Prerequisites
* rubygems

The installation of gem is depend on your operating system. Alternatively, you can download Gem through browser: [Ruby](https://www.ruby-lang.org/en/downloads/), and install rubygems manually.

```bash
# macOS

brew update
brew install ruby

# Ubuntu
sudo apt-get install ruby

# Arch
sudo pacman -S ruby

```

* bundler

```bash
gem install bundler
```
* jekyll
```bash
bundler install jekyll
```

* jekyll plugins

```bash
gem install jekyll-sitemap jekyll-feed jekyll-seo-tag jekyll-mermaid
```

### Installation

1. Fork this project on [github](https://github.com/akiritsu/pRoJEct-NeGYa), change project settings, and clone your own repository into your local disk.

```bash
git clone https://github.com/{{YOUR_USERNAME}}/{{YOUR_REPOSITORY}}.git
```

2. Change directory.

```bash
cd {{YOUR_REPOSITORY_DIR}}
```

### Personalize and Customize

#### _config.yml

Edit **_config.yml** with your own website information.

#### Collections

All your articles could be stored in this folder. You could create a new collection by creating a subfolder begin with a slash, and register the basic information in **_config.yml**. Here is an example:

```yaml
# Collections
collections:
  notes:
    output          : true
    permalink       : /:collection/:title/
    sort_by         : date
  portfolio:
    output          : true
    permalink       : /:collection/:title/
    order: # specify post order manually
      - portfolio3.md
      - portfolio2.md
      - portfolio1.md
  album:
    output          : true
    permalink       : /:collection/:title/
    sort_by         : date
```

All your articles would be shown by clicking **Archive** button in the header of your website.

#### Writing

Delete all sample collections under **./collections/**, and have fun in writing!

#### Comment

Create your own account in [Disqus.com](https://disqus.com/), and change the attribute "disqus_username" in **_config.yml**.

#### Test locally

Run command below, and access "127.0.0.1:4000" to test your website locally.

```bash
bundle exec jekyll serve
```

#### Front Matter

You can add many front matter to customize a page. For more information, visit official document: [https://jekyllrb.com/] (https://jekyllrb.com/docs/front-matter/)

```yaml
layout: post # page layout, must be one of layouts under src/_layouts
title: "Sample" # string
author: "your_name" # string
post_list: "cate" # whether to show post list under collections/_post, one of false, "cate", "date"
collection_list: true # true or false
toc: true # table of content, true or false
show_date: true # whether to show date, true or false
home_btn: true # whether to show home button, true or false
btn_text: true # whether to show button text, true or false
footer: true # whether to show footer, true or false
maximize: true # whether to show maximize button, true or false
encrypted_text: true # whether to enable encrypted text, true or false
publish: true # if you wish keep this page invisible, put false here
toc_level: 4 # the depth of toc, one of 1, 2, 3, 4, 5, 6
comment: ture # whether to show comment area
category: "sample" # string
date: 2019-5-25 # YYYY-MM-DD
excerpt: "This is excerpt." # string
abstract: "This is abstract. Abstract is blank by default." # string
```

## Roadmap

1. On-browser code execution teminal.
2. Code review mode.
3. Slide mode.
4. Rapid cheatsheet access.


<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE` for more information.


<!-- CONTACT -->
## Contact

DeerRIDER - [Email](mailto://deerrider666@outlook.com)

Project Link: [https://github.com/akiritsu/pRoJEct-NeGYa](https://github.com/akiritsu/pRoJEct-NeGYa)

[forks-shield]: https://img.shields.io/github/forks/akiritsu/pRoJEct-NeGYa.svg?style=flat-square
[forks-url]: https://github.com/akiritsu/pRoJEct-NeGYa/network/members
[stars-shield]: https://img.shields.io/github/stars/akiritsu/pRoJEct-NeGYa.svg?style=flat-square
[stars-url]: https://https://github.com/akiritsu/pRoJEct-NeGYa/stargazers
[issues-shield]: https://img.shields.io/github/issues/akiritsu/pRoJEct-NeGYa.svg?style=flat-square
[issues-url]: https://https://github.com/akiritsu/pRoJEct-NeGYa/issues
[license-shield]: https://img.shields.io/github/license/akiritsu/pRoJEct-NeGYa.svg?style=flat-square
[license-url]: https://https://github.com/akiritsu/pRoJEct-NeGYa/blob/master/LICENSE.txt
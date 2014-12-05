# docker-github-pages

Reproduces the GitHub Pages environment.

Project URL: https://github.com/fernandoacorreia/docker-github-pages

Repository URL: https://registry.hub.docker.com/u/fernandoacorreia/github-pages/

## Purpose

Provides an environment that reproduces GitHub Pages, allowing for local simulation of
how the site will be rendered.

## Contents

* Ruby 2.1.5
* github-pages 29

## Installed Gems

```
+-----------------------+---------+
| Gem                   | Version |
+-----------------------+---------+
| jekyll                | 2.4.0   |
| jekyll-coffeescript   | 1.0.0   |
| jekyll-sass-converter | 1.2.0   |
| kramdown              | 1.3.1   |
| maruku                | 0.7.0   |
| rdiscount             | 2.1.7   |
| redcarpet             | 3.1.2   |
| RedCloth              | 4.2.9   |
| liquid                | 2.6.1   |
| pygments.rb           | 0.6.0   |
| jemoji                | 0.3.0   |
| jekyll-mentions       | 0.1.3   |
| jekyll-redirect-from  | 0.6.2   |
| jekyll-sitemap        | 0.6.0   |
+-----------------------+---------+
```

## Usage

```
$ alias github-pages-preview='docker run --rm -v "$PWD:/src" -p 4000:4000 fernandoacorreia/github-pages'
$ github-pages-preview
```

Then preview the site by browsing [http://localhost:4000/](http://localhost:4000/).

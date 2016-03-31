# How to work in Minimal Mistakes Blogging Environment

[Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes/) is a blogging environment that works with the setup they have on GitHub. The intention is that users will generate content and have it served via their ID.github.io accounts. I selected MM because it had the most complete set of examples in its sample pages and blog posts (among the GitHub pages frameworks I looked at). It also had the most fully populated configuration file, which makes future customization easier.

At the moment, I am using this account to host online versions of Catechesis album pages.

## Tools used by the system

* Jekyll
* Octopress
* Kramdown

## Customization

* \_config.yml
  * site wide configuration
  * Things like title, icon, sidebar contents
* \_data/navigation.yml
  * Navigation links in the menu at the top of the page
* \_layouts
  * HTML boiler plate that content is inserted into.
* \_sass/variables.scss
  * Colors and fonts. The CSS stuff
* mathjax?

## Adding new content
Start by generating a blank page with the correct name. Then use a text editor (Atom is nice) to fill it with actual content. HOWEVER. I find that for a blog post, I don't get the title right unless I have written the post first. I often know the right title for the more structured "page" entries before I write them. That is probably because they are already copies of existing things.

* octopress new page DIRECTORY/
* octopress new page DIRECTORY/page
* octopress new post "post title"

## Reviewing content locally

First, build the site, stored in \_site. With the --incremental flag, you can get automatic rebuilding each time you make a change.

* jekyll build
* jekyll build --incremental

Then start a server which you can browse to to see the pages. Again, the --incremental flag will make new pages be generated and then served. The server address is [http://127.0.0.1:4000/](http://127.0.0.1:4000)

* jekyll serve
* jekyll serve --incremental

## Installing changes

In GitHub application on desktop:
* commit changes to master
* sync
* select the gh-pages branch
* in Branch menu, update from master
* sync

## Reviewing content on GitHub
[lindakukolich.github.io](lindakukolich.github.io)

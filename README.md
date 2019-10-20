# Tech blog

This blog use the static site generator Jekyll and the theme Long Haul.

## Setup

1. First you'll have to install [ruby](https://jekyllrb.com/docs/installation/macos/)
2. `gem install jekyll bundler`
3. `npm install` to install the dependencies
4. `bundle install` to install the Gems
5. `npm run serve` to run the website locally.

## Write an article

**/!\ You must switch to dev mode by commenting prod configuration and uncomment dev one. /!\\**

Article are stored in `_posts` folder. You must name your article as follow `YY-MM-DD-title.md`.
The article can be written in markdown (this is the manner to focus on) or in html. If needed, you'll find a cheatSheet [here](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet).

On the top of the file, there is an information section as following :

```
layout: post                        // Do not change that
title: 'Bienvenue sur notre blog'   // Title of the article
date: 2019-08-30                    // Writing date
image: touring.jpg                  // Image associated
author: Juliane                     // Author written at the end of the article
```

NB : The image must be put in the `assets/img` folder.

For more informations, you can read the md files in the folder `writing-tools`, it has some additionals infos for using Jekyll.

## Deploy the blog

**/!\ You must switch to prod mode by commenting dev configuration and uncomment prod one. /!\\**

When the develop branch has been merged into master,

1. Checkout on the gh-pages branch
2. Update it with master. For example : `git fetch && git reset --hard origin/master`
3. Push it
4. That's done !
   Github will automatically deploy the new version. You can see it [here](https://github.com/Schoolmouv-team/blog/deployments)

## Site Settings

The main settings can be found inside the `_config.yml` file:

- **title:** title of your site
- **description:** description of your site
- **url:** your url
- **paginate:** the amount of posts displayed on homepage
- **navigation:** these are the links in the main site navigation
- **social** diverse social media usernames (optional)
- **google_analytics** Google Analytics key (optional)

## License

This is [MIT](LICENSE) with no added caveats, so feel free to use this Jekyll theme on your site without linking back to me or using a disclaimer.

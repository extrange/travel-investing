# Our Investing Blog

![](static/images/index/money-pot.jpg)

There'll be separate sections for travel, investing, food etc.

We'll use [Markdown](https://guides.github.com/features/mastering-markdown/) for the writing syntax. It's easy to learn, looks like text, and the theming is applied separately so we can standardize.

Once we decide on a domain name we'll move this blog there.

I'm considering using [GatsbyJS](https://www.gatsbyjs.com/) to replace this theme ([Material for MkDocs](https://squidfunk.github.io/mkdocs-material/)), but I think this works for now.

If you're not sure how to push to git you can send me the markdown posts and photos and I'll post it for you.

Everything is version controlled with `git`, so don't worry about messing anything up - we can revert back to any point in time.

In case you're wondering, we can get free images from [unsplash.com](https://unsplash.com/).

## Technical

### Setup

Clone the repository with git: `git clone https://github.com/extrange/travel-investing.git`

Install packages from pipfile with `pipenv`: `pipenv install`

Start MkDocs development server: `mkdocs serve`

To build documentation: `mkdocs build`

### Project layout

    mkdocs.yml          # The configuration file.
    docs/   
        index.md        # The documentation homepage.
        posts/          # Posts here by category
            travel/ 
            investing/
            food/
        static/ 
            images/     # Images here. Probably stick to jpg for now.
            videos/     # Videos here
        ...             # Other markdown pages and files.

### Git Branches

`dev` is where we'll make draft changes.

`main` is the main branch, and upon pushing to `main`, a build will be triggered via github-actions on github-pages.
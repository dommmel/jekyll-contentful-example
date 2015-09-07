## Example Jekyll site using Contentful.com

This is a minimal example of a jekyll site using the [jekyll-contentful gem](https://github.com/dommmel/jekyll-contentful) to pull content from contentful.com at build time.

The example also demos the i18n features of the gem.

## Running the example

At contentful.com

1. Create a contentful.com account and a space (if you don't have one already)
2. Add a the "de-DE" locale to the space (Settings -> Locales)
3. Create a content type "Article".
4. Add a short text field with the ID "title" to the content type. Make sure to check "This field represents the Entry title" and  "enable localization of this field" on the field's settings page.
5. Add a long text field with the ID "body". Check the checkbox "enable localization of this field" on the field's settings page.
4. Create at least one entry (better more, and preferably translate them as well)

On your machine

1. Clone the repo and ``cd`` into the folder
2. Change ``_config.yml`` to include your Contentful API keys, Space ID, Content Type ID
3. Run ``bundle install`` to install the dependencies
4. Run ``bundle exec jekyll serve -w`` to build and serve the site
5. Visit [http://127.0.0.1:4000](http://127.0.0.1:4000) to view the site you just built.
![Termeul Banner](images/banner.png)

**Termeul** is a [Hugo](https://gohugo.io/) theme that is greatly inspired by [Risotto](https://github.com/joeroe/risotto).
It was made for my personal website [Eulenbude](https://eulenbu.de/).

Termeul was designed with the minimal requirements for my personal website in mind.
This theme is missing a lot of features that you might be used to from other themes.
However if all you want is a dead simple theme with no fluff, then Termeul might be for you.

# Install

Add this repository to the theme directory of your website, either as a submodule or by cloning it directly.
Either of these two lines will work.

```
git submodule add https://github.com/JoogsWasTaken/termeul.git themes/termeul
git clone https://github.com/JoogsWasTaken/termeul.git themes/termeul
```

Then add this theme to your `hugo.toml`.

```toml
theme = 'termeul'
```

# Configure

As mentioned, Termeul comes with very little fluff out of the box.
It is recommended that you disable the default taxonomies in your `hugo.toml` and enable the parsing of raw HTML tags in Hugo's default Markdown renderer like so.

```toml
disableKinds = ['taxonomy', 'term']

[markup.goldmark.renderer]
unsafe = true
```

See the [example configuration](exampleSite/hugo.toml) for reference.

## Favicon

I personally use [RealFaviconGenerator](https://realfavicongenerator.net/) for my own projects and I configured Termeul to work with its output.
Simply place the contents of the generated archive in the `static/` directory.

## Custom CSS and JS

You can add custom stylesheets and scripts by creating files in your static directory.
Termeul will automatically include `static/css/custom.css` and `static/js/custom.js` if present.

# License

MIT.

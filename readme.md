# wintersmith-showdown

[Showdown](https://github.com/lhagan/showdown) plugin for [wintersmith](https://github.com/jnordberg/wintersmith). Renders Markdown content using (a modified version of) Showdown instead of the default, [marked](https://github.com/chjj/marked). While slower to render, this enables lots of Markdown extras such as footnotes, tables, strikethrough, LaTeX math (via [MathML](http://www.mathjax.com)), and smart punctuation. This plugin also adds extremely inefficient code highlighting via `highlight.js`.

### install:

    npm install git@github.com:lhagan/wintersmith-showdown.git
  
then add `./node_modules/wintersmith-showdown/` to `config.json` like this:

    {
      "locals": {
        "url": "http://localhost:8080",
        "name": "The Wintersmith's blog",
        "owner": "The Wintersmith",
        "description": "-32°C ain't no problems!",
        "index_articles": 3
      },
      "plugins": [
        "./node_modules/wintersmith-showdown/"
      ]
    }
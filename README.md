# stipe

![agaric logo](https://agaric.net/img/agaric-64.png "agaric logo")

### about

- purpose:
    - personal blogging platform
    - an exercise after http://clojure-doc.org/articles/tutorials/basic_web_development.html (@ july 2017)
- deployed at:
    - [agaric.net](https://agaric.net)
- license:
    - [mit](https://raw.githubusercontent.com/agarick/stipe/master/LICENSE) (source code)
    - [cc by-nc-sa 4.0](https://agaric.net/about) (superposed content)

### operation

- Place all [markdown](https://github.com/yogthos/markdown-clj) files (eg. your individual blog posts) into a folder situated as `/db/`. The filenames should end in `.md` and the file contents can include [metadata](https://github.com/fletcher/MultiMarkdown/wiki/MultiMarkdown-Syntax-Guide#metadata), of which only `Title`, `Date`, and `Keywords` are used.
- Create `/config/master/config.edn` with [`:env`](https://github.com/agarick/stipe/blob/master/src/stipe/util.clj#L7) and [`:port`](https://github.com/agarick/stipe/blob/master/src/stipe/core.clj#L17) entries.
- Run `lein with-profile master run`

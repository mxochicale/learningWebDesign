[ Make a Static Website with Jekyll ](https://www.taniarascia.com/make-a-static-website-with-jekyll/)
---
https://github.com/taniarascia/startjekyll


$ mkdir www
$ cd www/
$ vim Gemfile
$ bundle install

```
.
.
.
Installing github-pages 151
Bundle complete! 1 Gemfile dependency, 74 gems now installed.
Use `bundle info [gemname]` to see where a bundled gem is installed.
Post-install message from html-pipeline:
-------------------------------------------------
Thank you for installing html-pipeline!
You must bundle Filter gem dependencies.
See html-pipeline README.md for more details.
https://github.com/jch/html-pipeline#dependencies
-------------------------------------------------

```


```
jekyll new startjekyll
cd startjekyll
git init
jekyll serve
```

```
firefox http://localhost:4000
```

ctrl-c

cd startjekyll

```
mkdir _includes && cd _includes
touch footer.html head.html header.html
```

```
cd ..
mkdir _layouts && cd _layouts
touch default.html page.html post.html
```

```
cd ..
mkdir _pages && cd _pages
touch 01_about.md 02_contact.md
```

```
mkdir _posts && cd _posts
```

```
_posts
I’m going to leave the post exactly as it is.
Delete about.md from the main directory, since we’ve put it in the _pages directory.
```

```
touch index.html
```

```
mkdir blog && cd blog
touch index.html
```


```
cd ..
mkdir css && cd css
touch main.scss
```

"Strange. I edited /css/main.sass and removed the two lines of "---" front
matter markers. It now compiles and serves."
https://github.com/dirkfabisch/mediator/issues/15#issuecomment-84524630


```
cd ..
mkdir _sass && cd _sass
touch _base.scss _syntax-highlighting.scss _layout.scss
```


```
jekyll serve

```


```
firefox  http://127.0.0.1:4000/
```




# ISSUES

```
$ jekyll serve
WARN: Unresolved specs during Gem::Specification.reset:
      listen (< 3.1, ~> 3.0)
WARN: Clearing out unresolved specs.
Please report a bug if this causes problems.
Configuration file: /home/map479-admin/startjekyll/_config.yml
            Source: /home/map479-admin/startjekyll
       Destination: /home/map479-admin/startjekyll/_site
 Incremental build: disabled. Enable with --incremental
      Generating...
                    done in 0.385 seconds.
 Auto-regeneration: enabled for '/home/map479-admin/startjekyll'
    Server address: http://127.0.0.1:4000/
  Server running... press ctrl-c to stop.

[2017-08-15 00:07:00] ERROR `/css/main.css' not found.
[2017-08-15 00:07:00] ERROR `/css/main.css' not found.

```


```
baseurl: "/startjekyll" # the subpath of your site, e.g. /blog
url: "https://mxochicale.github.io"
```

git remote add origin https://github.com/mxochicale/startjekyll.git
git checkout -b gh-pages
git add .
git commit -am "Initial commit"
git push origin gh-pages





Website
```
https://mxochicale.github.io/startjekyll/
```

# pingod-addons

Godot 4.1.1 docs, guides

TODO: make the workflow download the addons repo to build doxygen docs from. usually it builds from root directory on the solution.

---
## Live Docs

🌎 [pingod getting started](https://flippingflips.github.io/pingod-addons-docs/getting-started/) - Getting Started

🌎 [pingod-addons](https://FlippingFlips.github.io/pingod-addons-docs) - Home

---
## Class documentation

🌎 [pingod-addons - class list](https://flippingflips.github.io/pingod-addons-docs/html/annotated.html) - Online documentation built from this repository with DoxyGen

#### Doxygen

`doxygen Doxyfile`. This generates documentation from the files in the `addons` directory

#### Configuration in the DoxyFile

`PROJECT_NAME           = "PinGod (AddOns)"`

`INPUT                  = ./pingod-addons/addons`

`OUTPUT_DIRECTORY       = ./docs/public`

---
## Run docs local

From the repository directory run the docs folder with [Hugo](https://gohugo.io/). `hugo server -w -s docs`

```
Environment: "development"
Serving pages from memory
Running in Fast Render Mode. For full rebuilds on change: hugo server --disableFastRender
Web Server is available at http://localhost:59492/pingod-addons/ (bind address 127.0.0.1)
Press Ctrl+C to stop
```


`choco install hugo-extended` [Chocolatey](https://chocolatey.org/):




## Building docs offline

The site requires [Hugo](https://gohugo.io/) to build or run. The Doxygen file configuation is built to the `docs/public/html` directory



This site uses the [hugo-theme-techdoc](https://github.com/thingsym/hugo-theme-techdoc) as a submodule and this can be updated by running:

`git submodule foreach git pull origin main`

## HUGO tech docs site
---

The docs directory is a HUGO website generator. You can run this locally and make edits to the markdown.

`hugo server -w` - This will run server and watch for file changes

Build the hugo site into a directory named public:

`hugo --minify`

### Generate doxygen class references locally
---


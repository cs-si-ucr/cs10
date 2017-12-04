# CS10
This website is used as a resource for the CS10 SI sessions at UC Riverside. Lecture and lab material can be accessed here to be used during sessions.

## How to Edit

* Each page is written in Markdown and can be found inside the `docs` folder.
  * Each file corresponds to a new webpage
* The `mkdocs.yml` file describes the structure of the generated site
  * You will map the Markdown files with the titles used on the site
* You will need to install mkdocs `sudo apt install mkdocs`
* Use `mkdocs serve` to deploy the website locally


## How to Deploy

* `mkdocs gh-deploy`
  * This will push the generated site to the `gh-pages` branch
  * You can then access the website at [http://cs-si-ucr.github.io/cs10](http://cs-si-ucr.github.io/cs10)

## Cool Resources

[Markdown reference](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
[MkDocs documentation](http://www.mkdocs.org/)

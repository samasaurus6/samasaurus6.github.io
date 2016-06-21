# Polymaps website

## Local checking environment

### Windows am too dumb for this version

* Download [latest hugo stable version](https://github.com/spf13/hugo/releases) and put hugo.exe in tools directory 
* run watch.bat
* Do your changes, use `http://localhost:1313` to preview changes
* Commit changes in git and push/sync

## Changing content

`{name}` should be dashed-cased (eg. `Superawesome Thing` -> `superawesome-thing`)

### Adding people

* Run in command line: `tools\hugo new people/{name}.md`
* Edit page content in `content\people\{name}.md`
* Avatar must be `content\people\{name}.png`
* Set `weight: {n}` for ordering
* To add more social links copy-paste `[[social]]` blocks, icons should match [font-awesome](http://fontawesome.io/icons/)

### Adding maps

* Run in command line: `tools\hugo new maps/{name}.md`
* Edit page content in `content\maps\{name}.md`. To separate description and rest of the page content use `<!--more-->`
* Icon must be `content\maps\{name}\icon.png`
* Background on map page must be `content\maps\{name}\background.jpg`
* Other images should be added to `content\maps\{name}\images\` folder, can be named anything. Reccomended 16:9 jpg
* `maps/authors` should match author's page's title (with casing)
* To add more download links copy-paste `[[download]]` blocks

### Adding projects

* Run in command line: `tools\hugo new projects/{name}.md`
* Edit page content in `content\projects\{name}.md`. To separate description and rest of the page content use `<!--more-->`
* Thumbnail must be `content\projects\{name}\thumb.jpg` (A square)
* Other images should be added to `content\projects\{name}\images\` folder, can be named anything. Reccomended 16:9 jpg
* `projects/authors` should match author's page's title (with casing)
* To add more links copy-paste `[[link]]` blocks, icons should match [font-awesome](http://fontawesome.io/icons/)

# VSCode Markdown Editor
  
This is a markdown editor for [VSCode](https://code.visualstudio.com/ ).
  
It's configured specifically for working with Github Flavored Markdown (GFM), but it can be retooled to work for any purpose like creating PDFs.
  
## Install
  
1. Clone this repo or just copy this file structure to its own `Workspace`.
   - If you want to run this setup in an existing project, remember to include the `Workspace` and Markdownlint settings.
2. Install [Pandoc](https://pandoc.org/installing.html ) on your machine.
   - The easiest way is to [download the installer](https://github.com/jgm/pandoc/releases/tag/3.2 ).
3. Install the following extensions on VSCode:
   - [Markdown All in One](https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one ) \- adds a bunch of cool shortcuts
   - [Markdown Checkboxes](https://marketplace.visualstudio.com/items?itemName=bierner.markdown-checkbox ) \- adds support for github checkboxes
   - [Markdown Emoji](https://marketplace.visualstudio.com/items?itemName=bierner.markdown-emoji ) \- adds support for emoji :unicorn:
   - [Markdown Footnotes](https://marketplace.visualstudio.com/items?itemName=bierner.markdown-footnotes ) \- adds support for citations
   - [Markdown PDF](https://marketplace.visualstudio.com/items?itemName=yzane.markdown-pdf ) \- allows conversion to PDF, HTML, PHG, or JPG
   - [Markdown Preview Enhanced](https://marketplace.visualstudio.com/items?itemName=shd101wyy.markdown-preview-enhanced ) \- adds a preview pane with a bunch of options on right-click
   - [Markdown Preview Mermaid Support](https://marketplace.visualstudio.com/items?itemName=bierner.markdown-mermaid ) \- adds support for mermaid diagrams
   - [markdownlint](https://marketplace.visualstudio.com/items?itemName=DavidAnson.vscode-markdownlint ) \- a very handy markdown linter
   - [Code Spell Checker](https://marketplace.visualstudio.com/items?itemName=streetsidesoftware.code-spell-checker ) \- a spell checker for VSCode. It also checks the spelling of a variety programming languages, but it mostly just clutters up your code with a bunch of squiggly lines.
4. Restart VSCode
  
## How to use
  
Click `⌘` + `k` then `v` on a Mac, or `ctrl` + `k` then `v` in Windows to open the enhanced preview pane. `Right click` to bring up the menu. Choose `export -> Save as Markdown` to save as GFM.
  
Define `Workspace` settings in the `.vscode` directory.
  
```json
{
	"editor.insertSpaces": false,
	"editor.quickSuggestions": {
		"comments": "on",
		"strings": "on",
		"other": "on"
	},
	"editor.formatOnSave": false,
	"pandoc.htmlOptString": "-s -f gfm -t html5 --css=css/style.css",
	"markdown-pdf.styles": [".//css//style.css"]
}
```
  
 Include or exclude linting rules in `.markdownkint.json`
  
 ```json
{
	"default": true,
	"MD007": true,
	"MD004": false,
	"no-hard-tabs": false,
	"line-length": false,
	"MD041": false
}
 ```
  
## Features
  
Import images
![markdown logo on blue background](assets/markdown-logo-on-a-blue-background.png )
  
Make Tables
| Red  |Blue   | Green|
|---:|---:|---:|
|  1 | 2  |3 |
  
Add emojis
:fairy_woman:	:mermaid:	:lotus_position: 	:hippopotamus: :poop: :clown_face:
  
...and so much more
  
Have fun and happy marking down! 	:alien:
  
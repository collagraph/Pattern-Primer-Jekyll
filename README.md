# Collagraph verions off Pattern-Primer by adactio

Forked from the [Jekyll version](https://github.com/opattison/Pattern-Primer-Jekyll) by [Opattison](https://github.com/opattison) which is a fork of the [original Pattern-Primer for PHP by adactio (Jeremy Keith)](https://github.com/adactio/Pattern-Primer)

## Pattern Primer

This is a design communication, testing and process tool.

Create little snippets of markup and save them to the "patterns folder" (called _posts in Jekyll). The pattern primer will generate a list of all the patterns in that folder. You will see the pattern rendered as HTML. You will also get the source displayed in a textarea.

We're also using this to store markup and css patterns that can help with rapid development of standard website components.

## How to use it

1. If you haven't already, [install Jekyll](http://jekyllrb.com/).
2. Clone this repo.
3. Copy your CSS file to css/global.css (replacing adactio's stock CSS) *or* copy your own CSS to the css directory and direct a link in the HTML to that file.
4. Create your own HTML snippets and add them to the `_posts` folder.
5. Run the command `jekyll serve` and open <localhost:4000> in your browser.

**One quirk of using this in Jekyll** (or at least the quick way I created it) is that the patterns are stored in the "_posts" folder. Every post must have identical front matter that looks like this:

```
---
layout: pattern
---
```

... and each file must be named `yyyy-mm-dd-title.html`. The date tag is arbitrary, but this will determine where it appears in order on the index. The default is set to 0001-01-01 for the packaged HTML snippets, but anything named newer than that will appear at the bottom of the list.
# MarkdownHighlighting
Sublime Text 3 Markdown grammar with scope names to provide some basic highlighting in all (legacy) color schemes, including classics like [Tomorrow](https://packagecontrol.io/packages/Tomorrow%20Color%20Schemes).

Most color schemes don't support the markdown syntax provided by the default package, or even packages like Markdown Extended. This package provides some basic hooks for markdown syntax highlighting in any color scheme.

Based on the latest version of the [default Markdown package](https://github.com/sublimehq/Packages/tree/master/Markdown), and adds highlighting for Github Flavoured Markdown style fenced code blocks from 
[Markdown Extended](https://github.com/jonschlinkert/sublime-markdown-extended).

Before  
![](https://raw.githubusercontent.com/braver/Markdown-Highlighting/master/before.png)

After  
![](https://raw.githubusercontent.com/braver/Markdown-Highlighting/master/after.png)


## Tips

You can create [Syntax Specific settings](https://www.sublimetext.com/docs/3/settings.html) settings to further improve the editing experience for Markdown files. 

Adding these settings will create a centered view of 80 characters wide, which makes reading and writing Markdown that much easier:

```json
"draw_centered": true,
"word_wrap": "true",
"wrap_width": 80,
```

If you use double trailing spaces to indicate line breaks, you might not want to trim white space:

```json
"trim_trailing_white_space_on_save": false,
```

Spell checking is super nice to have in Markdown. This enables it for everything except URLS and in-line code:

```json
"spell_check": true,
"spelling_selector": "meta.paragraph - markup.underline.link - markup.raw, markup.quote - markup.underline.link.markdown - markup.raw"
```

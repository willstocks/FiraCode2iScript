# Fira Code v5.2 + iScript
A mish-mash of Fira Code v5.2 and iScript

I was originally using https://github.com/kencrocken/FiraCodeiScript, however it hasn't been updated in a while and [Fira Code](https://github.com/tonsky/FiraCode) has had a LOAD of really useful updates to it since that I wanted to make use of.

Originally this was Fira Code v2 + iScript, however Fira Code has now had multiple releases since. At some point, I may apply a _minor_ rename to the font to remove the Two/2 so the naming is a bit more... relevant!


## Installation
This is _really_ simple to install - download the three `.ttf` files and install them on your system. 

Then, launch whatever code editor you use and apply `Fira Code Two iScript` as your font family.

In VSCode, I use (with fallbacks for multiple machines): 

```json
"editor.fontFamily": "Fira Code Two iScript, FiraCode-Retina, Fira Code Retina, Fira Code, Consolas, 'Courier New', monospace",
```

I then apply the following in `settings.json` as well to enable italics:

```js
"editor.tokenColorCustomizations": {
    "textMateRules": [
        {
            "scope": [
                "comment",
                "constant", //String, Number, Boolean…, this, super
                "keyword", //import, export, return…
                "markup.italic",
                "meta.selector",
                "storage.modifier", //static keyword
                "storage.type",
                "storage.type.class.js", //class keyword
                "variable.language",
            ],
            "settings": {
                "fontStyle": "italic",
            }
        },
        {
            "scope": [
                //following will be excluded from italics (VSCode has some defaults for italics which aren't amazingT)
                "invalid",
                "keyword.operator",
                "constant.numeric.css",
                "keyword.other.unit.px.css",
                "constant.numeric.decimal.js",
                "constant.numeric.json"
            ],
            "settings": {
                "fontStyle": ""
            }
        }
    ]
}
```

## Screenshots
Coming soon...

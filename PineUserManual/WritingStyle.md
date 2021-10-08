# Writing Style

### Rules for capitalization in titles
* Capitalize the first word of the title
* Capitalize all proper nouns

### Quotation marks
Documentation uses American style which considers a double quotes are the default ones. Single quotes are used if nested in the double ones. For example: 
* Joe said, "Will you marry me?"
* Joe smiled and said, "Jenny said 'yes' when I asked her to marry me."

### Inline markup
* One asterisk: `*text*` for emphasis (italics),
* Two asterisks: `**text**` for strong emphasis (boldface), and
* Two backquotes: &#96;&#96;text&#96;&#96; for inline code samples.

### Special unicode characters

There is a set of macros in file [isonum.txt](http://docutils.sourceforge.net/docs/ref/rst/definitions.html).
For example for &rarr; (RIGHTWARDS ARROW) use `|rarr|` macro. 
For example:
```
..    include:: <isonum.txt>
Indicators |rarr| Built-ins
```

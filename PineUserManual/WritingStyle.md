# Writing Style

We use U.S. English style and spelling standards, unless otherwise specified here.

## Style

### Tone
- Use "We" — never "I"
- We try to mix the assertive tone fitting to documentation with more engaging language such as:
  - Let's look at an example where...



## Typographic conventions



### Capitalization of titles
* Capitalize only the first word of the title



### Quotation marks
We use straight double quotes in RST files, which get converted to opening/closing double curly quotes in the HTML content.
American style which considers a double quotes are the default ones. Single quotes are used if nested in the double ones. For example: 
* Joe said, "Will you marry me?"
* Joe smiled and said, "Jenny said 'yes' when I asked her to marry me."



### Bold face
We use bold (marked up as ``**text**``) to indicate emphasis, e.g.:
- This line must be the **last** one in the local block.


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

# Writing Style

### Table of Contents

- [Style](#style)
  - [Tone](#tone)
- [Typographic conventions](#typographic-conventions)
  - [Capitalization of titles](#tone)
  - [Quotation marks](#quotation-marks)
  - [Bold](#bold)
  - [Italics](#italics)
  - [Monospace](#monospace)
  - [Em dash](#em-dash)


We use U.S. English style and spelling standards, unless otherwise specified here.

## Style

### Tone
Use "We" — never "I"

We try to mix the assertive tone fitting to documentation with more engaging language such as:
- Let's look at an example where...



### Presentation of examples
When we present code examples, we use the following order:

1. A brief introduction.
2. The screenshot, if there is one.
3. The code.
4. The explanatory segment starting with "Note that:", followed by bullet points.

See an example [here](https://www.tradingview.com/pine-script-docs/en/v5/concepts/Colors.html#conditional-coloring).



## Typographic conventions



### Capitalization of titles
Capitalize only the first word of the title



### Quotation marks
We use straight double quotes in RST files, which get converted to opening/closing double curly quotes in the HTML content.
American style which considers a double quotes are the default ones. Single quotes are used if nested in the double ones. For example: 
* Joe said, "Will you marry me?"
* Joe smiled and said, "Jenny said 'yes' when I asked her to marry me."



### Bold
We use bold (marked up as ``**bold text**``) to indicate emphasis, e.g.:
- This line must be the **last** one in the local block.


### Italics
We use italics (marked up as ``*italic text*``) when:
1. Introducing concepts, e.g.:
- [...] where "const" is considered a *weaker* form than "input", for example, and "series" *stronger* than "simple".



### Monospace
We use monospace (marked up as &#96;&#96;monospace text&#96;&#96;) for inline Pine code segments **that are not a Pine built-in variable or function name** e.g.:
- This line must be the **last** one in the local block.



### Em dash
We use a space on each side of Em dashes:
- Providing a selection of color presets in your inputs — rather than a single color that can be changed — can help color-challenged users. 




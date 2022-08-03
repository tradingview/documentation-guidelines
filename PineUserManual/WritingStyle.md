# Writing Style



### Table of Contents

- [Style](#style)
  - [Tone](#tone)
  - [Presentation of examples](#presentation-of-examples)
- [Typographic conventions](#typographic-conventions)
  - [Capitalization of titles](#tone)
  - [Quotation marks](#quotation-marks)
  - [Bold](#bold)
  - [Italics](#italics)
  - [Monospace](#monospace)
  - [Em dash](#em-dash)
  - [Thousands separator](#thousands-separator)

We use U.S. English style and spelling standards, unless otherwise specified here.



## Style



### Tone
Use "We" — never "I".

We try to mix the assertive tone fitting to documentation with more engaging language such as:
- Let's look at an example where...



### Presentation of examples
When we present code examples, we use the following order:

1. An introductory paragraph ending with a colon (":"). The paragraph's text should provide the information required for readers to understand the big picture of what they will be seeing in the screenshot or code. Leave details to the explanatory segment in point 4.
2. The screenshot, if there is one.
3. The code.
4. The explanatory segment starting with "Note that:", followed by bullet points.
    If there is only one note, use one paragraph, beginning its first sentence with "Note that".

See an example [here](https://www.tradingview.com/pine-script-docs/en/v5/concepts/Colors.html#conditional-coloring).



## Typographic conventions



### Pine keywords
See [the section on Pine keywords in the RST Guidelines](https://github.com/tradingview/documentation-guidelines/blob/main/PineUserManual/RSTGuidelines.md#pine-keywords).



### Capitalization of titles
Capitalize only the first word of the title and headings: "Chart information", "Other timeframes and data".



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
1. Referring to user interface components:
    - Use the "Settings" dialog box to modify the script's inputs, visual attributes, or visiblity.
    - Users of your script can change its input values with the "Settings/Inputs" tab.
    - You can load scripts on your chart with the "Indicators & Strategies" button situated above the chart.
    - Scripts define alert events; actual alerts must be created using the chart's "Create Alert" dialog box.
1. Referring to form-type pairs, or forms, or types (see the ["Forms and types" section of the RST Guidelines](https://github.com/tradingview/documentation-guidelines/blob/main/PineUserManual/RSTGuidelines.md#forms-and-types)).


### Monospace
We use monospace (marked up as &#96;&#96;monospace text&#96;&#96;) for inline Pine code segments **that are not a Pine built-in variable or function name** e.g.:
- This line must be the **last** one in the local block.



### Em dash
Contrary to standard practices in English, we use a space on each side of Em dashes. 
The EM dash is not very wide in the Trebuchet MS font used in the HTML rendition of the User Manual;
the spaces on each side make them more prominent:
- Providing a selection of color presets in your inputs — rather than a single color that can be changed — can help color-challenged users. 



### Thousands separator
We use a comma for the thousands separator with values starting at 10,000. We write "1000" but "10,000".

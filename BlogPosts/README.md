# Pine Blog Posts



### Table of Contents

- [Style](#style)
- [Structure](#structure)
- [Typographic conventions](#typographic-conventions)


We use U.S. English style and spelling standards, unless otherwise specified here.



## Style

Focus on what's in it for users: what they can do with the new feature, and how.

Our writing style should be the usual TV style: no frills, no bs, engaging, sometimes funny, and to the point. If you are unsure, ask for help from James.



## Structure

Use this stucture for all posts:

1. A catchy title (ask help from James and Laurie if needed)
1. An short introductory paragraph (two or three sentences) summarizing the new feature AND mentioning its most important impact from a user's point of view.
1. One or more sub-sections explaining how to use the feature, with a script example and a screenshot if needed.
1. Our standard two closing paragraphs.
1. The "What's new" notification text to be used for the blog post.


### Code examples

Our code examples should:

- Follow the recommendations from our [Style guide](https://www.tradingview.com/pine-script-docs/en/v5/writing/Style_guide.html)
- Ideally demonstrate something that can be of practical use to traders.
- Be complete, i.e., compilable. If a demonstration would require an inordinately long script, then we can use only the relevant code lines.

Favor readability over conciseness.


### Closing paragraphs

We use the following text to close all blog posts:

```
To stay informed of new Pine features, keep an eye on our Pine User Manual's [Release notes](https://www.tradingview.com/pine-script-docs/en/v4/Release_notes.html).
The [PineCoders](https://www.tradingview.com/u/PineCoders/) account also broadcasts updates from its [Squawk Box](https://t.me/PineCodersSquawkBox) Telegram channel, 
[Twitter account](https://twitter.com/PineCoders), and from the Pine Script public chat on TradingView.

We hope you find this highly-requested feature useful. Please keep giving  us your feedback and suggestions for improvement — we build TradingView for you, and we’re always keen to hear from you.
```



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




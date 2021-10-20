# Pine Blog Posts



### Table of Contents

- [Process](#process)
- [Writing Style](#writing-style)
- [Structure](#structure)
  - [Code Examples](#code-examples)
  - [Closing Paragraphs](#closing-paragraphs)
  - [Screenshots](#screenshots)
- [Typographic Conventions](#typographic-conventions)
  - [Pine Keywords](#pine-keywords)
  - [Inline Code](#inline-code)
  - [Block Code](#block-code)
  - [Capitalization of Titles](#capitalization-of-titles)
  - [UI Component Names](#ui-component-names)
  - [Double Quotation Marks](#double-quotation-marks)
  - [Structure](#structure)
  - [Structure](#structure)
  - [Structure](#structure)
  - [Structure](#structure)


We use U.S. English style and spelling standards, unless otherwise specified here.


## Process

Blog posts should be well-planned and coordinated with the rollout of the feature:

- Although it's not a requirement, it's useful for users if we can include links to published scripts using the feature. This entails that we coordinate with PineCoders and give them at least a week to come up with worthwhile example scripts.
- If you cannot think of useful code examples, ask PineCoders in the or Luc.

Because it's always useful for users to see actual scripts using the feature, we should ideally try to coordinate with PineCoders to have some 



## Writing Style

Focus on what's in it for users: what they can do with the new feature, and how.

Our writing style should be the usual TV style: no frills, no bs, engaging, sometimes humorous, and to the point. If you are unsure, ask for help from James.



## Structure

Use this stucture for all posts:

1. A **catchy title** (ask help from James and Laurie if needed)
1. A **short introductory paragraph** (two or three sentences) summarizing the new feature AND mentioning its most important impact from a user's point of view.
1. One or more **sub-sections** explaining how to use the feature, with a script example and a screenshot for each sub-section, if needed.
1. When possible, **links to script publications** using the new feature should be included.
3. Our standard [closing paragraphs](#closing-paragraphs).
4. The "What's new" **notification text** to be used for the blog post.


### Code Examples

Our code examples should:

- Follow the recommendations from our [Style guide](https://www.tradingview.com/pine-script-docs/en/v5/writing/Style_guide.html).
- Ideally demonstrate something that can be of practical use to traders, as opposed to code merely illustrating the feature and not useful in a trading context.
- Be complete, i.e., compilable. If a full demonstration would require an inordinately long script, then we can use only the relevant code lines.

Favor readability over conciseness.


### Closing Paragraphs

We use the following text to close all blog posts:

> To stay informed of new Pine features, keep an eye on our Pine User Manual's [Release notes](https://www.tradingview.com/pine-script-docs/en/v4/Release_notes.html).
The [PineCoders](https://www.tradingview.com/u/PineCoders/) account also broadcasts updates from its [Squawk Box](https://t.me/PineCodersSquawkBox) on Telegram, 
its [Twitter account](https://twitter.com/PineCoders), and from the Pine Script public chat on TradingView.
>  
> We hope you find this highly-requested feature useful. Please keep sending us your feedback and suggestions for improvement. We build TradingView for you, and we’re always keen to hear from you.

You can pick up the standard text to paste it in your blog post from [this doc](https://docs.google.com/document/d/1PUtJFrLIkYmUKwIwmxwqX0JipjFVek6Qs20QiXuQK98/edit?usp=sharing).



### Screenshots



## Typographic Conventions



### Pine Keywords
Whenever we use a Pine keyword that has an entry in the Reference Manual, we link it to its entry, which accomplishes two things:
- It helps readers by providing easy access to the Reference Manual.
- It formats the keyword in blue, which makes it stand out.

Also:
- Always use ``()`` to suffix function names, e.g., [math.ceil()](https://www.tradingview.com/pine-script-reference/v5/#fun_math{dot}ceil).
- When referring to a family of functions, such as ``array.*()``, use [inline code](#inline-code) markup.

Use the standard linking feature in Google docs to mark up keywords; the links will be preserved in the post. Linked keywords will look like this in the published posts:

![.](images/Keywords.png "Pine keywords")



### Inline Code
We use backticks to wrap inline code when it is not a keyword that can be linked to Reference Manual entry, e.g.:
> Use the ```confirm``` parameter to...
  Our ```if barstate``` line...
  The ``request.*()`` functions fetch data from other contexts than the chart's.

Text wrapped in backticks will be converted to monospace by Alexander:

![.](images/Monospace.png "Monospace")



### Block Code
We format block code in a monospace font in the post's document.



#### Capitalization of Titles
Contrary to our [Writing Guidelines for the Pine User Manual](https://github.com/tradingview/documentation-guidelines/tree/main/PineUserManual), we capitalize titles in blog posts. You can use a tool like [Capitalize My Title](https://capitalizemytitle.com/) to produce correctly capitalized titles.



### UI Component Names
We wrap UI component names in double quotes:
- Use the "Settings" dialog box to modify the script's inputs, visual attributes, or visiblity.
- Users of your script can change its input values with the "Settings/Inputs" tab.
- You can load scripts on your chart with the "Indicators & Strategies" button situated above the chart.
- Scripts define alert events; actual alerts must be created using the chart's "Create Alert" dialog box.



### Double Quotation Marks
Besides UI component names, we use double quotes when referring to:
- The title of a publication on TradingView or elsewhere, as in:
  > The "CAGR" indicator...
- Form-type pairs, or forms, or types (see the ["Forms and types" section of the RST Guidelines](https://github.com/tradingview/documentation-guidelines/blob/main/PineUserManual/RSTGuidelines.md#forms-and-types)).



### Bold
We use bold to indicate emphasis, e.g.:
- This line must be the **last** one in the local block.



### Italics
We use italics when:
1. Introducing concepts, e.g.:
    - [...] where "const" is considered a *weaker* form than "input", for example, and "series" *stronger* than "simple".



### Em dash
Contrary to standard practices in English, we use a space on each side of Em dashes. 
The EM dash is not very wide in the Trebuchet MS font used in the HTML rendition of the User Manual;
the spaces on each side make them more prominent:
- Providing a selection of color presets in your inputs — rather than a single color that can be changed — can help color-challenged users. 



## Examples

[Pine Scripts Are Now Interactive](https://www.tradingview.com/blog/en/pine-scripts-are-now-interactive-27147/)

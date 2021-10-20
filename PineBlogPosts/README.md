# Pine Blog Posts



### Table of Contents

- [Process](#process)
- [Writing Style](#writing-style)
- [Structure](#structure)
- [Typographic conventions](#typographic-conventions)
  - [Pine keywords](#pine-keywords)
  - [Inline code](#inline-code)
  - [Block code](#block-code)
  - [Capitalization of titles](#capitalization-of-titles)
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


### Code examples

Our code examples should:

- Follow the recommendations from our [Style guide](https://www.tradingview.com/pine-script-docs/en/v5/writing/Style_guide.html).
- Ideally demonstrate something that can be of practical use to traders, as opposed to code merely illustrating the feature and not useful in a trading context.
- Be complete, i.e., compilable. If a full demonstration would require an inordinately long script, then we can use only the relevant code lines.

Favor readability over conciseness.


### Closing paragraphs

We use the following text to close all blog posts:

> To stay informed of new Pine features, keep an eye on our Pine User Manual's [Release notes](https://www.tradingview.com/pine-script-docs/en/v4/Release_notes.html).
The [PineCoders](https://www.tradingview.com/u/PineCoders/) account also broadcasts updates from its [Squawk Box](https://t.me/PineCodersSquawkBox) on Telegram, 
its [Twitter account](https://twitter.com/PineCoders), and from the Pine Script public chat on TradingView.
>  
> We hope you find this highly-requested feature useful. Please keep sending us your feedback and suggestions for improvement. We build TradingView for you, and we’re always keen to hear from you.

You can pick up the standard text to paste it in your blog post from [this doc](https://docs.google.com/document/d/1PUtJFrLIkYmUKwIwmxwqX0JipjFVek6Qs20QiXuQK98/edit?usp=sharing).



## Typographic conventions



### Pine keywords
Whenever we use a Pine keyword that has an entry in the Reference Manual, we link it to its entry, which accomplishes two things:

- It helps readers by providing easy access to the Reference Manual.
- It formats the keyword in blue, which makes it stand out.

Linked keywords will look like this in the published posts:

![.](images/Keywords.png "Pine keywords")



### Inline code
We use backticks to wrap inline code when it is not a keyword that can be linked to Reference Manual entry, e.g.:
- Use the ```confirm``` parameter to...
- Our ```if barstate``` line...

Backticks will be converted by the publisher of the blog post into monospace that will look like this in the post:

![.](images/Monospace.png "Monospace")



### Block code
We format block code in a monospace font in the post's document.



#### Capitalization of titles
Contrary to our User Manual guidelines, we capitalize titles. You can use a tool like [Title Capitalization & Title Case Converter Tool - Capitalize My Title](https://capitalizemytitle.com/) to apply the proper rules to your titles.



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



### Em dash
Contrary to standard practices in English, we use a space on each side of Em dashes. 
The EM dash is not very wide in the Trebuchet MS font used in the HTML rendition of the User Manual;
the spaces on each side make them more prominent:
- Providing a selection of color presets in your inputs — rather than a single color that can be changed — can help color-challenged users. 



## Examples

[Pine Scripts Are Now Interactive](https://www.tradingview.com/blog/en/pine-scripts-are-now-interactive-27147/)

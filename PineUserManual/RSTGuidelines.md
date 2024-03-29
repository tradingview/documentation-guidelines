# RST guidelines

### Table of Contents

- [RST Filenames](#rst-filenames)
- [Automatic table of contents](#automatic-table-of-contents)
- [Images](#images)
- [Code examples](#code-examples)
- [Pine keywords](#pine-keywords)
- [Forms and types](#forms-and-types)
- [Internal References](#internal-references)
- [UI names](#ui-names)
- [Keyboard shortcuts](#keyboard-shortcuts)



## RST Filenames
Take a page title, replace all spaces with underscores (`_`), remove all punctuation (except dashes, `-`), add `.rst` extension.
A page with this title, for example:
```
User-defined functions
======================
```
Should be saved on disk as `User-defined_functions.rst`.


## Automatic table of contents
Use the `contents`  directive after the page's title. You can specify the number of levels needed with ``:depth:``:
```
User-defined functions
======================

.. contents:: :local:
    :depth: 2
```



## Images

Keep the following in mind:
- Screenshots **must always have an even number of pixels in height and width**. This produces better clarity when images are scaled.
- Design your chart so what we are trying to illustrate is most prominent, e.g.:
    - If candles are not required, consider using bars.
    - If candles are required but the focal point of the chart, consider using 20% opacity on their normal colors to make them less prominent.
    - Use a horizontal and vertical zoom factor that suits what you are showing.
- Unless specified otherwise in the RST ``image`` directive, images are scaled to occupy the full width of the HTML frame. Size screenshots accordingly, so they are wider than high. This will avoid having square screenshots of a dialog box, for example, appearing huge in the rendered pages.
- Use the ShareX macro that produces our standard blue border with rounded corners.
- Disable any color-adapting utilities like "f.lux" for your screenshots.

#### References
The easiest way to place images is by using: 
```
.. image:: images/Colors-UsingColors-1.png
```
which requires only one line and no references at the end of the file, as is the cas when the ``|Colors-UsingColors-1|`` syntax is used.

#### Location
Images should always be placed in the ``images`` directory in the same directory as the RST file.

#### Naming

Image names should use the following nomenclature: ``PageName-SectionName-[x/text].ext`` where ``x`` can be a sequential digit, or ``text`` can be used to further qualify the image. Examples: ``Arrays-HistoryReferencing.png``, ``Arrays-ManipulatingArrays-Concat.png``, ``Colors-CalculatingColors-1.png``.

#### Screenshots

Images should ideally have an even number of pixels in height and width.

Screenshots should be taken using the English version of the platform and the ShareX macro that Tim has created to add a thin blue border with rounded corners.



## Code examples

Code snippets should conform to our [Style guide](https://www.tradingview.com/pine-script-docs/en/v4/Style_guide.html).

We use the following syntax to format code:

```
[text]::

    //@version=5
    indicator("")
    plot(na)
```

where ``[text]`` is optional text.



## Pine keywords

When referring to a function, always include ``()`` after its name. This helps distinguish between the `ta.tr` variable and the `ta.tr()` function, for example.

Use external links like the following one for ALL Pine keywords with an entry in the Reference Manual: ``indicator()``, ``plot.style_line``, ``if``, ``na``, ``true``, etc.::

```
`ta.tr <https://www.tradingview.com/pine-script-reference/v5/#var_ta{dot}tr>`__
`ta.tr() <https://www.tradingview.com/pine-script-reference/v5/#fun_ta{dot}tr>`__
```

When Pine keywords must be included in headings, we use visible backticks to wrap the keywords because monospace doesn't apparently work well in headings. We escape the backtick with a backslash. Extend the level marks under the title to include the last backtick:

```
Using \`bgcolor()\`
-------------------
```



## Forms and types

We enclose form and type names in straight double quotes: "const", "int", "float", "simple color".

We can use *type* to mean the "form-type" pair, but it's preferable to avoid it when we can. To do so, we can use workarounds like:

```
The ``length`` parameter requires a "simple int" argument.
A "series float" variable cannot be used there.
```



## Internal References

When linking to other pages or sections of the User Manual, use *anchored references*.
Anchored references require a definition in the target page, 
and the use of ``:ref:`` directives when linking to the anchor from any RST file.

##### To refer to pages

Use the "PagePagename" style for page anchor names. 
Place the anchor definition on the very first line of the page.

1. Define the ``PagePagename`` anchor in the page you will be linking **to**, by using:
    ```
    `.. _PageTypeSystem:`
    ```
    so the page's beginning looks like:
    ```
    `.. _PageTypeSystem:`

    Type system
    ===========

    .. contents:: :local:
        :depth: 3



    Introduction
    ------------
    ```

2. To refer to that anchor from any RST file, use the ``:ref:`` directive:
    ```
    :ref:`link_text <PageTypeSystem>`
    ```
    ``link_text`` is the link's visible text in the doc. It is mandatory for the reference to work.
    Note that the leading underscore in the definition of the anchor must **not** be present when we link to the anchor.
    Also note that some ``link_text`` is **mandatory**, and that a space **must** follow it before the ``<PageTypeSystem>`` part.
    
    Text using the reference could look like:
    
    ```
    The type system is intimately linked to Pine's :ref:`execution model <PageExecutionModel>`.
    ```

##### To refer to sections

Use the "PagePagename_SectionName" style for section anchor names, where the ``PagePagename`` prefix is the page's anchor name.
If a page anchor does not already exist, you should create one to ensure it uses the anchor name you will be using as a prefix in your section anchor names.

To refer to the "Z-index" section of the "Colors" page, use `.. _PageColors_ZIndex:`:

1. Define your anchor above the section's title, leaving one empty line after it:
    ```
    Previous section's last paragraph's line, followed by three empty lines.
    
    
    
    .. _PageColors_ZIndex:

    Z-index
    ^^^^^^^

    First line of the "Z-index" section. 
    ```

2. To refer to that anchor from any RST file, use the ``:ref:`` directive:
    ```
    :ref:`link_text <PageColors_ZIndex>`
    ```


## UI names

We enclose UI element names in double quotes. Use a slash to separate elements in menus paths.

This applies to dialog boxes names, tab names, button names, menu selections, etc.:

```
Open the "Create Alert" dialog box using ALT + A
The script's "Settings/Inputs" tab
Use the Editor's "Open/My script..." menu.
```


## Keyboard shortcuts

Use the ``:kbd:`` directive and lowercase letters for the key names:

```
Use :kbd:`ctrl` + :kbd:`click` / :kbd:`cmd` + :kbd:`click` on Pine keywords to launch the popup Reference Manual.
It provides an auto-complete feature that you can activate with :kbd:`ctrl` + :kbd:`space` / :kbd:`cmd` + :kbd:`space`.
```


### Special unicode characters
There is a set of macros in file [isonum.txt](http://docutils.sourceforge.net/docs/ref/rst/definitions.html).
For example for &rarr; (RIGHTWARDS ARROW) use `|rarr|` macro. 
For example:
```
..    include:: <isonum.txt>
Indicators |rarr| Built-ins
```

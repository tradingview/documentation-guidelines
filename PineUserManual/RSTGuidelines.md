# RST guidelines




## Images

### References
The easiest way to place images is by using: 
```
.. image:: images/Colors-UsingColors-1.png
```
which requires only one line and no references at the end of the file, as is the cas when the ``|Colors-UsingColors-1|`` syntax is used.

### Location
Images should always be placed in the ``images`` directory in the same directory as the RST file.

### Naming

Image names should use the following nomenclature: ``PageName-SectionName-[x/text].ext`` where ``x`` can be a sequential digit, or ``text`` can be used to further qualify the image. Examples: ``Arrays-HistoryReferencing.png``, ``Arrays-ManipulatingArrays-Concat.png``, ``Colors-CalculatingColors-1.png``.

### Screenshots

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

When referring to a function, always include "()" after its name. This helps distinguish between the `ta.tr` variable and the `ta.tr()` function.

If we are referring to a function, variable or operator for which a Reference Manual entry exists, we create a link for it using:

```
`ta.tr <https://www.tradingview.com/pine-script-reference/v5/#var_ta{dot}tr>`__
`ta.tr() <https://www.tradingview.com/pine-script-reference/v5/#fun_ta{dot}tr>`__
```

When Pine keywords must be included in headings, we use visible backticks to wrap the keywords because monospace doesn't apparently work well in headings:

```
Using \`bgcolor()\`
-------------------
```



## Pine forms and types

We enclose form and type names in straight double quotes: "const", "int", "float", "simple color".

We can use *type* to mean the "form-type" pair, but it's preferable to avoid it when we can. To do so, we can use workarounds like:

```
The ``length`` parameter requires a "simple int" argument.
A "series float" variable cannot be used there.
```



## References to other pages or sections

### Within the User Manual

When linking to other pages or sections of the User Manual, use *anchored references*. They require two steps:

1. Define the anchor in the page you will be linking **to**, by using:
    ```
    `.. _PageName_SectionName:`
    ```
    so the page's beginning looks like:
    ```
    Type system
    ===========

    .. contents:: :local:
        :depth: 3

    .. include:: <isonum.txt>


    Introduction
    ------------
    ```

2. Link to the anchor using:
    ```
    :ref:`link_text <PageName_SectionName>`
    ```
    ``link_text`` is the link's visible text in the doc. It is mandatory for the reference to work.
    Note that the leading underscore in the definition of the anchor must not be present when we link to the anchor.
    Also note that some ``link_text`` is necessary, and that a space must follow it before the ``<PageName_SectionName>`` part.

#### Anchor naming conventions

##### For pages

We use "PagePagename" for the page anchor, which is placed at the top of the file, e.g., `.. _PageTypeSystem:`. 
This allows us to refer to that page using `` :ref:`link text <PageTypeSystem>` ``.

##### For page sections

We use "PagePagename_SectionName" for section anchors, where "PagePagename" is the page the section belongs to,  
e.g., `.. _PageColors_ZIndex:` for the "Z-Index" section of the page on Colors.



## UI names (dialog boxes, buttons, tabs, etc.)

We enclose UI element names in double quotes. Use a slash to separate elements in menus paths:

```
Open the "Create Alert" dialog box using ALT + A
The script's "Settings/Inputs" tab
Use the Editor's "Open/My script..." menu.
```

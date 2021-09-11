# RST guidelines

## References

When linking to other pages or sections of the User Manual, use *anchored references*. They require two steps:

1. Define the anchor using `.. _anchorText:`
2. Link to the anchor using `` :ref:`link text <anchorText>` `` if you want "link text" to be the link's visible text, or `` :ref:`<anchorText>` `` if you want to use the text from the header immediately following the anchor in the linked file.

### Anchor naming

#### For pages

We use "PagePagename" for the page anchor, which is placed at the top of the file, e.g., `.. _PageTypeSystem:`. 
This allows us to refer to that page using `` :ref:`link text <PageTypeSystem>` ``.

#### For page sections

We use "PagePagename_SectionName" for section anchors, where "PagePagename" is the page the section belongs to, e.g., `.. _PageColors_ZIndex:` for the "Z-Index" section of the page on Colors.

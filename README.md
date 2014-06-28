---
layout: default
title: Readme
---

---

# README

Repository for FLOSS network, systems, and infrastructure related designs. 

## Markdown and Image Formats

Please use basic markdown (including GFM(Github Flavoured Markdown) http://github.github.com/github-flavored-markdown/ and a minimum of **both** an optimised for web image such as .jpg / .png **and** its associated editable source file in .svg or .uml (or if all that is available then a .graffle or .vsd). Such that the file size limits on github apply in this repository please use simple shapes, lines, and text to keep your diagram file sizes under 10MiB. This will also have the byproduct of incentivising the removal of vendor bitmaps and colours on complex diagrams forcing the authors to rethink how to convey meaning in black and white simplicity. If you can not diagram with simple and standard shapes then perhaps you are not modelling for the widest audience possible (which is in fact a goal i.e. both technical and non-technical audiences).

## Dynamic Page Generation

All that is required is to create a design named "ond-0000X.md" in markdown such that the index 'x' is not taken already and then submit a git pull request with your file(s). Your .md file once created with the following additional few lines of headers:

    --- 
    layout: default 
    title: ond-0000x
    tag: designs
    type: designs
    ---

...will additionally cause a runtime dynamic .html file to be generated by Github such that URLs can be linked and displayed via the webpage including a forthcoming auto-generated list of designs.


## Reminder

As always, please share, comment, contribute in a helpful manner where critiscism is constructive. Collaboration and community is key. Energy flows.

## License 

Please see the associated __LICENSE.md__ file in this directory which outlines more about the CC0 1.0 Universal (CC0 1.0) 
Public Domain Dedication https://creativecommons.org/publicdomain/zero/1.0/

- Added mcLapply functionality to parallelize tasks using Snow and Parallel package in R
- Thanks @http://www.sfu.ca/~sblay/R/snow.html for such a helpful implementation of parallel computing in R

<!-- README.md is generated from README.Rmd. Please edit that file -->
rvest
=====
Overview
--------

The most important functions in rvest are:

-   Create an html document from a url, a file on disk or a string containing html with `read_html()`.

-   Select parts of a document using css selectors: `html_nodes(doc, "table td")` (or if you've a glutton for punishment, use xpath selectors with `html_nodes(doc, xpath = "//table//td")`). If you haven't heard of [selectorgadget](http://selectorgadget.com/), make sure to read `vignette("selectorgadget")` to learn about it.

-   Extract components with `html_tag()` (the name of the tag), `html_text()` (all text inside the tag), `html_attr()` (contents of a single attribute) and `html_attrs()` (all attributes).

-   (You can also use rvest with XML files: parse with `xml()`, then extract components using `xml_node()`, `xml_attr()`, `xml_attrs()`, `xml_text()` and `xml_tag()`.)

-   Parse tables into data frames with `html_table()`.

-   Extract, modify and submit forms with `html_form()`, `set_values()` and `submit_form()`.

-   Detect and repair encoding problems with `guess_encoding()` and `repair_encoding()`.



PureBASIC Syntax Highlighting
=============================

When it comes to publishing code, PureBASIC language is still unsupported in most syntax highlighting tools. I’ve created PB syntax files for highlight.js and highlight, and working toward the creation of syntax files for Pygments and Kate.

<!-- #toc -->
-   [In This Repo](#in-this-repo)
    -   [Highlight](#highlight)
-   [Available Highlighters](#available-highlighters)
    -   [Backend HTML Highlighters](#backend-html-highlighters)
        -   [GeSHi — Generic Syntax Highlighter](#geshi--generic-syntax-highlighter)
    -   [In-Browser Highlighters](#in-browser-highlighters)
        -   [highlight.js](#highlightjs)
-   [Needed Highlighters](#needed-highlighters)
    -   [Pygments](#pygments)

<!-- /toc -->
In This Repo
============

Highlight
---------

-   [/highlight/](./highlight/)

This repo hosts the project page of the PureBASIC language definition and color theme for Highlight syntax highligther.

Written by Tristano Ajmone, public domain.

Available Highlighters
======================

Backend HTML Highlighters
-------------------------

### GeSHi — Generic Syntax Highlighter

-   <http://qbnz.com/highlighter/>

GeSHi is a GPL licensed syntax highlighter for HTML written in PHP, originally conceived for the [phpBB](http://phpbb.net/) forum system but now supporting integration in a wide variety of CMSs, as well as being a PHP (&gt; 4.3.0) library.

GeSHi 1.0 nativaly supports PureBASIC — syntax file created by GuShH (Gustavo Julio Fiorenza), ©2009, licensed under GNU 2 (or above):

-   <https://github.com/GeSHi/geshi-1.0/blob/master/src/geshi/purebasic.php>

In-Browser Highlighters
-----------------------

JavaScript tools capable of syntax highlighting code directly into the webpage.

### highlight.js

The author of this project has created the PureBASIC syntax files for the in-browser syntax highlighter highlight.js:

-   https://highlightjs.org
-   https://github.com/tajmone/highlight.js

There is also an unofficial “PureBASIC enhanced release”, which emulates 100% the PureBASIC native IDE syntax coloring — maintained on a separate fork because it doesn’t comply to the highlight.js guidelines:

-   https://github.com/tajmone/highlight.js/tree/PureBASIC

This repo will soon host pre-built versions of highlight.js “PureBASIC enhanced releases”, with different combinations of language syntaxes, to cover common usage, along with instructions and examples.

Needed Highlighters
===================

There is a need to create PureBASIC syntax highligthing for some popular highlighters that are commonly used in publishing toolchains.

Pygments
--------

-   <http://pygments.org/>

Pygments is a very popular Python (2/3) syntax highlighter. By creating a PureBASIC syntax file for Pygments it would allow PB syntax support for the following apps/services (among many others):

-   [Hugo](https://gohugo.io/) — a powerful cross-platform static site generator written in Go, distributed as a single standalone binary executable. Converts markdown source files to an HTML5 site and serves it locally; can also deploy it online. It uses Pygments as the default syntax highlighter. For more info, [see Hugo documentation](https://gohugo.io/extras/highlighting).

    NOTE: Currently PureBASIC code can be highlighted on Hugo via highlight.js (client-side) instead of Pygments (server-side); but Pygments offers finer control (line numbers, highlighting certain lines, and more).



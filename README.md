# Pandoc Workflows

[Pandoc](https://pandoc.org/) can be pretty useful as a general purpose templating system that allows you to write your content in [Markdown](https://en.wikipedia.org/wiki/Markdown) files and create various documents such as articles, slideshows, and websites from it. This repository contains some example files that demonstrate this approach and can be used as template for new projects.

**Advantages**: The content is reasonably separate from its presentation, allowing to focus on the structure of the content when writing it. Furthermore, this approach works very well with version control.
**Disadvantages**: It can be hard to change certain aspects of the output documents and that it is difficult to collaborate with people who are not comfortable working with plain-text files.

## Companion Tools

**[Makefiles](https://www.gnu.org/software/make/manual/html_node/index.html)** are useful to store the commands that build the documents and can also be used to download Pandoc itself. Since `make` is available on most Linux systems it often doesn’t even need to be installed explicitly. Alternatives such as [just](https://github.com/casey/just) may be preferable if you prefer a more modern and simple tool.

**[entr](https://github.com/eradman/entr)** provides a convenient way to rerun a build command whenever the input files have changed. You still have to reload the browser though for web-based output, unless you use a browser extension or local web server that implement live reload functionality.

## Further Resources

The [Pandoc manual](https://pandoc.org/MANUAL.html) has many relevant details. The section on Pandoc’s Markdown is particularly useful.

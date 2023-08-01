# Pandoc for Presentations

Presentations are built with `make slides` or simply `make`. Alternatively the Pandoc command can be executed directly. Arguments in the form `--variable=key:value` can also be moved to the YAML metadata block at the beginning of the Markdown file.

Whether the slides are built as a one-dimensional or two-dimensional presentation can be controlled by the `--slide-level` argument passed to Pandoc. If it is omitted, the slide level is selected based on which heading levels have content as children, which can be a bit confusing. Any [reveal.js option](https://revealjs.com/config/) can be set as a variable either in the YAML metadata or in the arguments of the Pandoc command.

Slides can be saved as PDF using the method [described here](https://revealjs.com/pdf-export/). Alternatively, you can also create a PDF-version of the document using Pandoc, which would ignore the slide styling and build the document with LaTeX instead.

The sample image is from [unDraw](https://undraw.co/), which has a great collection of vector images that can be used without attribution (even for commercial use) and can be remixed to create custom, high-quality illustrations.

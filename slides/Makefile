# Presentation setup (could be moved to the Markdown file, but since it is more
# output-related it is included here)
width = 1600
height = 900
theme = white # see https://revealjs.com/themes/

# By default, Pandoc includes a link to a hosted version of the reveal.js
# library in the HTML output. Downloading a local copy makes the build a bit
# more complex, but avoids relying on an internet connection to view the
# presentation.
revealjs-version = 4.4.0
revealjs = .cache/reveal.js-${revealjs-version}
${revealjs}:
	wget -O revealjs.tar.gz https://github.com/hakimel/reveal.js/archive/refs/tags/${revealjs-version}.tar.gz
	mkdir -p "$@"
	tar -xzf revealjs.tar.gz --strip-components=1 --directory="$@"
	rm revealjs.tar.gz

.DEFAULT_GOAL = slides
.PHONY: slides watch

slides: presentation.html

watch:
	ls *.md | entr make slides

presentation.html: presentation.md | ${revealjs}
	pandoc --standalone --to=revealjs --variable=revealjs-url:${revealjs} \
		--variable=width:${width} --variable=height:${heigth} --variable=theme:${theme} \
		--slide-level=2 --output="$@" "$<"

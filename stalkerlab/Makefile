.PHONY: all print
all print: stalkerlab.pdf

stalkerlab.pdf: stalkerlab.tex preamble.tex literature.bib
stalkerlab.pdf: contents.tex aims.tex literature.tex


.PHONY: clean
clean:
	${RM} stalkerlab.pdf


INCLUDE_MAKEFILES=../makefiles
include ${INCLUDE_MAKEFILES}/tex.mk
include ${INCLUDE_MAKEFILES}/doc.mk

SRC+=		diffpriv-preamble.tex diffpriv.bib
SRC+=		abstract.tex diffpriv-content.tex

.PHONY: all
all: diffpriv-notes.pdf

diffpriv-notes.pdf: llncs biblatex-lncs
diffpriv-notes.pdf: diffpriv-notes.tex ${SRC}


.PHONY: all
all: diffpriv-slides.pdf

diffpriv-slides.pdf: diffpriv-slides.tex ${SRC}


.PHONY: clean
clean:
	${RM} diffpriv-notes.pdf
	${RM} diffpriv-slides.pdf


INCLUDE_MAKEFILES=../makefiles
include ${INCLUDE_MAKEFILES}/tex.mk

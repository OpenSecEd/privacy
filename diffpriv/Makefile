SRC+=		preamble.tex diffpriv.bib
SRC+=		abstract.tex contents.tex

#.PHONY: all
#all: notes.pdf
#
#notes.pdf: notes.tex ${SRC}


.PHONY: all
all: slides.pdf

slides.pdf: slides.tex ${SRC}


.PHONY: clean
clean:
	${RM} notes.pdf
	${RM} slides.pdf


INCLUDE_MAKEFILES=../makefiles
include ${INCLUDE_MAKEFILES}/tex.mk

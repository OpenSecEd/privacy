.PHONY: all
all: diffpriv-notes.pdf diffpriv-slides.pdf

SRC+=		diffpriv-preamble.tex diffpriv.bib
SRC+=		abstract.tex diffpriv-content.tex

diffpriv-notes.pdf: llncs biblatex-lncs
diffpriv-notes.pdf: diffpriv-notes.tex ${SRC}

diffpriv-slides.pdf: diffpriv-slides.tex ${SRC}


INCLUDE_MAKEFILES=../makefiles
include ${INCLUDE_MAKEFILES}/tex.mk

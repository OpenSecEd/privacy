SRC+=		preamble.tex diffpriv.bib
SRC+=		abstract.tex contents.tex

DEPENDS+= 	bibsp.sty beamer-didactic.sty

#.PHONY: all
#all: notes.pdf
#
#notes.pdf: notes.tex ${SRC} ${DEPENDS}


.PHONY: all
all: slides.pdf

slides.pdf: slides.tex ${SRC} ${DEPENDS}


.PHONY: clean
clean:
	${RM} notes.pdf
	${RM} slides.pdf


INCLUDE_MAKEFILES=../makefiles
include ${INCLUDE_MAKEFILES}/tex.mk
INCLUDE_BIBSP=../bibsp
include ${INCLUDE_BIBSP}/bibsp.mk
INCLUDE_BEAMERDIDACTIC=../beamer-didactic
include ${INCLUDE_BEAMERDIDACTIC}/beamer-didactic.mk
